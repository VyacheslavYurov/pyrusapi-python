# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.21.0] - 2023-10-03
### Added
- source_type field added into CreateCatalogRequest and CatalogResponse

## [2.20.0] - 2023-08-15
### Added
- roles fields added: avatar_id, external_avatar_id

## [2.19.0] - 2023-07-11
### Added
- members field added: external_avatar_id

## [2.18.0] - 2023-07-06
### Added
- list/get/create/update members
- members fields added: status, avatar_id
- method set_avatar 

## [2.17.0] - 2023-07-06
### Added
- get a single role

## [2.16.0] - 2023-03-13
### Added
- get/add/update roles

## [2.15.0] - 2023-03-13
### Added
- 'edit_note_id' property in :obj:models.requests.TaskCommentRequest request

## [2.14.0] - 2023-02-17
### Added
- form permissions api

## [2.13.0] - 2022-12-01
### Added
- 'cancel_due' property in :obj:models.requests.TaskCommentRequest request

## [2.12.0] - 2022-06-22
### Added
- 'due_filter' property in :obj:models.requests.TaskListRequest request

## [2.11.0] - 2022-06-15
### Added
- get_announcements method

## [2.10.0] - 2022-06-06
### Added
- item_count parameter for get_registry method

## [2.9.1] - 2022-06-02
### Fixed
- get_task_list method response type fix

## [2.9.0] - 2022-04-28
### Added
- operations with Announcement entities

## [2.8.0] - 2022-04-20
### Added
- 'modified_before', 'modified_after' properties in :obj:models.requests.TaskListRequest request

## [2.7.0] - 2022-04-11
### Added
- 'reply_note_id' property in :obj:models.entities.TaskComment entity
- 'due_date' property in :obj:models.entities.TaskHeader entity

## [2.6.0] - 2022-03-30
### Added
- 'code' property in FormFieldInfo and _get_named_fields method

## [2.5.0] - 2021-02-15
### Added
- 'task_ids' argument in FormRegisterRequest

## [2.4.0] - 2021-01-21
### Added
- 'include_inactive' argument in get_contacts and get_profile methods

## [2.3.0] - 2021-01-20
### Added
- 'mentions' property in :obj:models.entities.TaskComment entity

## [2.2.0] - 2022-01-18
### Added
-  Get calendar request

## [2.1.0] - 2022-01-10
### Added
-  Get inbox request

## [2.0.0] - 2021-12-30
### Added
- Support for custom channel and sms sending via external channel 

### Changed
- 'сhannel' property type changed to :obj:models.entities.Channel
- Renamed 'deletedOrClosed' property to 'deleted_or_closed'

## [1.35.0] - 2021-12-27
### Added
-  Support for skipping user satisfaction poll in task comments
-  Return 'multiple_choice' in 'Catalog' form field

## [1.34.0] - 2021-12-21
### Added
-  Get profile request

### Changed
-  Department catalog id property added in 'Organization' entity

## [1.33.0] - 2021-12-17
### Changed
-  Fixed custom handler

## [1.32.0] - 2021-12-09
### Changed
-  Removed 'rfc6266' dependency

## [1.31.0] - 2021-04-29
### Changed
-  Changed auth request method from GET to POST

## [1.30.0] - 2021-03-02
### Added
-  'Folder' property in GetForm response

## [1.29.0] - 2020-11-16
### Added
- 'DepartmentId' and 'DepartmentName' properties in entity of 'Person' in 'contacts' response

## [1.28.0] - 2020-11-09
### Added
- 'DeletedOrClosed' property in GetForm response

## [1.27.0] - 2020-10-27
### Added
- support for reading and writing subscribers in task comments

## [1.26.1] - 2020-06-26
### Changed
- bugfix

## [1.26.0] - 2020-06-26
### Added
- new external source channels

## [1.25.0] - 2020-04-17
### Added
- support for reading and writing spent time in task comments

## [1.24.0] - 2020-04-16
### Added
- support for attaching files by id or by url

## [1.23.0] - 2019-10-24
### Added
- support for reading and writing multiple values in catalog field
- root_id for files with version

## [1.22.0] - 2019-09-04
### Added
- allow to write value to catalog field by id or by name

## [1.21.0] - 2019-09-03
### Added
- support sending comments to external channel (email)

## [1.19.0] - 2019-05-16
### Added
- This CHANGELOG file.
- Return decimal_places for form field number.
- added scheduling task to date with utc time.
- fill step number for form task approvals

### Changed
- Fixed FormField serialization. You can now copy all fields from TaskResponse change some of them and pass to the TaskCommentRequest.
- Fixed parsing filename from Content-Disposition header on file download.
- Fixed creation_date field value.
