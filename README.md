import 'dart:convert';

import 'package:json_annotation/json_annotation.dart';
import 'package:simple_app/features/Profile/data/models/user_model.dart';
import 'package:simple_app/features/addPermit/data/model/user_data_model.dart';
import 'package:simple_app/features/courses/data/model/course_unit.dart';
import 'package:simple_app/features/courses/domain/entity/course_entity.dart';

part 'course_model.g.dart';



@JsonSerializable()
class CourseModel {
  @JsonKey(name: "courseId")
  int courseId;
  @JsonKey(name: "code")
  String code;
  @JsonKey(name: "courseNameFL")
  String courseNameFl;
  @JsonKey(name: "courseNameSL")
  String courseNameSl;
  @JsonKey(name: "categoryId")
  int categoryId;
  @JsonKey(name: "quizeId")
  dynamic quizeId;
  @JsonKey(name: "smsProfileId")
  int smsProfileId;
  @JsonKey(name: "textMessageProfileId")
  int textMessageProfileId;
  @JsonKey(name: "tags")
  List<String> tags;
  @JsonKey(name: "isAutoAnnounce")
  bool isAutoAnnounce;
  @JsonKey(name: "description")
  dynamic description;
  @JsonKey(name: "units")
  List<dynamic> units;
  @JsonKey(name: "hasQuiz")
  bool hasQuiz;
  @JsonKey(name: "noOfTrainees")
  int noOfTrainees;
  @JsonKey(name: "trainerId")
  int trainerId;
  @JsonKey(name: "searchedValue")
  dynamic searchedValue;
  @JsonKey(name: "totalDuration")
  int totalDuration;
  @JsonKey(name: "smsProfileVM")
  dynamic smsProfileVm;
  @JsonKey(name: "textMessageProfileVM")
  dynamic textMessageProfileVm;
  @JsonKey(name: "courseCategoryVM")
  CourseCategoryVm courseCategoryVm;
  @JsonKey(name: "countFiles")
  int countFiles;
  @JsonKey(name: "countVideos")
  int countVideos;
  @JsonKey(name: "totalProgress")
  int totalProgress;
  @JsonKey(name: "imageGUID")
  dynamic imageGuid;
  @JsonKey(name: "isStarted")
  bool isStarted;
  @JsonKey(name: "scheduleManagerVM")
  dynamic scheduleManagerVm;
  @JsonKey(name: "trainerVM")
  dynamic trainerVm;
  @JsonKey(name: "entryUserId")
  int entryUserId;
  @JsonKey(name: "entryUser")
  User entryUser;
  @JsonKey(name: "entryDate")
  DateTime entryDate;
  @JsonKey(name: "entryDateString")
  dynamic entryDateString;
  @JsonKey(name: "lastUpdateUserId")
  dynamic lastUpdateUserId;
  @JsonKey(name: "lastUpdateUser")
  dynamic lastUpdateUser;
  @JsonKey(name: "lastUpdateDate")
  dynamic lastUpdateDate;
  @JsonKey(name: "lastUpdateDateString")
  dynamic lastUpdateDateString;
  @JsonKey(name: "isActive")
  bool isActive;
  @JsonKey(name: "isRemoved")
  bool isRemoved;
  @JsonKey(name: "enrolmentUser")
  User enrolmentUser;
  @JsonKey(name: "tenantId")
  int tenantId;

  CourseModel({
    required this.courseId,
    required this.code,
    required this.courseNameFl,
    required this.courseNameSl,
    required this.categoryId,
    required this.quizeId,
    required this.smsProfileId,
    required this.textMessageProfileId,
    required this.tags,
    required this.isAutoAnnounce,
    required this.description,
    required this.units,
    required this.hasQuiz,
    required this.noOfTrainees,
    required this.trainerId,
    required this.searchedValue,
    required this.totalDuration,
    required this.smsProfileVm,
    required this.textMessageProfileVm,
    required this.courseCategoryVm,
    required this.countFiles,
    required this.countVideos,
    required this.totalProgress,
    required this.imageGuid,
    required this.isStarted,
    required this.scheduleManagerVm,
    required this.trainerVm,
    required this.entryUserId,
    required this.entryUser,
    required this.entryDate,
    required this.entryDateString,
    required this.lastUpdateUserId,
    required this.lastUpdateUser,
    required this.lastUpdateDate,
    required this.lastUpdateDateString,
    required this.isActive,
    required this.isRemoved,
    required this.enrolmentUser,
    required this.tenantId,
  });

  factory CourseModel.fromJson(Map<String, dynamic> json) => _$CourseModelFromJson(json);

  Map<String, dynamic> toJson() => _$CourseModelToJson(this);
}

@JsonSerializable()
class CourseCategoryVm {
  @JsonKey(name: "courseCategoryId")
  int courseCategoryId;
  @JsonKey(name: "code")
  dynamic code;
  @JsonKey(name: "courseCategoryNameFL")
  String courseCategoryNameFl;
  @JsonKey(name: "courseCategoryNameSL")
  String courseCategoryNameSl;
  @JsonKey(name: "parentId")
  dynamic parentId;
  @JsonKey(name: "description")
  dynamic description;
  @JsonKey(name: "parent")
  dynamic parent;
  @JsonKey(name: "entryUserId")
  int entryUserId;
  @JsonKey(name: "entryUser")
  User entryUser;
  @JsonKey(name: "entryDate")
  DateTime entryDate;
  @JsonKey(name: "entryDateString")
  dynamic entryDateString;
  @JsonKey(name: "lastUpdateUserId")
  dynamic lastUpdateUserId;
  @JsonKey(name: "lastUpdateUser")
  dynamic lastUpdateUser;
  @JsonKey(name: "lastUpdateDate")
  dynamic lastUpdateDate;
  @JsonKey(name: "lastUpdateDateString")
  dynamic lastUpdateDateString;
  @JsonKey(name: "isActive")
  bool isActive;
  @JsonKey(name: "isRemoved")
  bool isRemoved;
  @JsonKey(name: "enrolmentUser")
  User enrolmentUser;
  @JsonKey(name: "tenantId")
  int tenantId;

  CourseCategoryVm({
    required this.courseCategoryId,
    required this.code,
    required this.courseCategoryNameFl,
    required this.courseCategoryNameSl,
    required this.parentId,
    required this.description,
    required this.parent,
    required this.entryUserId,
    required this.entryUser,
    required this.entryDate,
    required this.entryDateString,
    required this.lastUpdateUserId,
    required this.lastUpdateUser,
    required this.lastUpdateDate,
    required this.lastUpdateDateString,
    required this.isActive,
    required this.isRemoved,
    required this.enrolmentUser,
    required this.tenantId,
  });

  factory CourseCategoryVm.fromJson(Map<String, dynamic> json) => _$CourseCategoryVmFromJson(json);

  Map<String, dynamic> toJson() => _$CourseCategoryVmToJson(this);
}

@JsonSerializable()
class User {
  @JsonKey(name: "userId")
  int userId;
  @JsonKey(name: "personNameFL")
  String personNameFl;
  @JsonKey(name: "personNameSL")
  String personNameSl;
  @JsonKey(name: "personId")
  int personId;
  @JsonKey(name: "personTypeId")
  int personTypeId;

  User({
    required this.userId,
    required this.personNameFl,
    required this.personNameSl,
    required this.personId,
    required this.personTypeId,
  });

  factory User.fromJson(Map<String, dynamic> json) => _$UserFromJson(json);

  Map<String, dynamic> toJson() => _$UserToJson(this);
}


