import 'dart:convert';
import 'package:dartz/dartz.dart';
import 'package:simple_app/core/baseRepo/base_repo.dart';
import 'package:simple_app/core/network/apiResponse/api_response.dart';
import 'package:simple_app/core/utls/urls.dart';
import 'package:simple_app/features/courses/data/model/course_model.dart';

import '../../../../core/network/dio_helper.dart';
import '../../../../core/network/exceptions/failures.dart';
import 'courses_remote_data_source.dart';

class CoursesRemoteDataSourceImpl extends NetworkService implements CoursesRemoteDataSource {


  @override
  Future<Either<Failure,List<CourseModel>>> getCourses() async {
    return await exceptionHandler(
      () async {
    APiResponse<dynamic> response = await dioHelper.getData(URLs.coursesList);
    List<dynamic> responcedata = response.data;
    print("API Response1: ${responcedata.toString()}");
    // final responceObj = json.decode(responcedata) as List<dynamic>;
    List<CourseModel> result = responcedata.map((obj) => CourseModel.fromJson(obj)).toList();
    return result;
      },
    );
  }

// bool _isRequestSuccess(int statusCode) {
//   return statusCode >= 200 && statusCode < 300;
// }
}
