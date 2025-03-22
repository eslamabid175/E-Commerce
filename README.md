I/flutter ( 1357): -----------------ELearning/private/course/search
I/flutter ( 1357): {type: https://tools.ietf.org/html/rfc9110#section-15.5.1, title: One or more validation errors occurred., status: 400, errors: {id: [The value 'search' is not valid.]}, traceId: 00-0e70d221e98945dfd6f8ace08b4cddd9-2c2dd0ce5b3895fa-00}
[Response: https://watcharea-aramco02.3i-vision.com/Way/ELearning/private/course/search] {"type":"https://tools.ietf.org/html/rfc9110#section-15.5.1","title":"One or more validation errors occurred.","status":400,"errors":{"id":["The value 'search' is not valid."]},"traceId":"00-0e70d221e98945dfd6f8ace08b4cddd9-2c2dd0ce5b3895fa-00"}
[log] 400
I/flutter ( 1357): {type: https://tools.ietf.org/html/rfc9110#section-15.5.1, title: One or more validation errors occurred., status: 400, errors: {id: [The value 'search' is not valid.]}, traceId: 00-0e70d221e98945dfd6f8ace08b4cddd9-2c2dd0ce5b3895fa-00}
I/flutter ( 1357): Some thing went wrong
I/flutter ( 1357): #0      DioHelper.handleResponse (package:simple_app/core/network/dio_helper.dart:282:7)
I/flutter ( 1357): #1      DioHelper.getData (package:simple_app/core/network/dio_helper.dart:248:12)
I/flutter ( 1357): <asynchronous suspension>
I/flutter ( 1357): #2      CoursesRemoteDataSourceImpl.getCourses.<anonymous closure> (package:simple_app/features/courses/data/remoteData/courses_remote_data_source_impl.dart:19:37)
I/flutter ( 1357): <asynchronous suspension>
I/flutter ( 1357): #3      NetworkService.exceptionHandler (package:simple_app/core/baseRepo/base_repo.dart:14:20)
I/flutter ( 1357): <asynchronous suspension>
I/flutter ( 1357): #4      CoursesRemoteDataSourceImpl.getCourses (package:simple_app/features/courses/data/remoteData/courses_remote_data_source_impl.dart:17:12)
I/flutter ( 1357): <asynchronous suspension>
I/flutter ( 1357): #5      CoursesListRepoImpl.getCoursesList (package:simple_app/features/courses/data/repoImp/courses_list_repo_impl.dart:17:11)
I/flutter ( 1357): <asynchronous suspension>
I/flutter ( 1357): #6      GetCoursesListUsecase.getCoursesListUc (package:simple_app/features/courses/domain/usecase/get_courses_list_usecase.dart:8:46)
I/flutter ( 1357): <asynchronous suspension>
I/flutter ( 1357): #7      CourseListCubit.getC
[log] {type: https://tools.ietf.org/html/rfc9110#section-15.5.1, title: One or more validation errors occurred., status: 400, errors: {id: [The value 'search' is not valid.]}, traceId: 00-0e70d221e98945dfd6f8ace08b4cddd9-2c2dd0ce5b3895fa-00}
I/flutter ( 1357): mogss Some thing went wrong
[log] {type: https://tools.ietf.org/html/rfc9110#section-15.5.1, title: One or more validation errors occurred., status: 400, errors: {id: [The value 'search' is not valid.]}, traceId: 00-0e70d221e98945dfd6f8ace08b4cddd9-2c2dd0ce5b3895fa-00}
