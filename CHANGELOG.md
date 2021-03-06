# Changelog

### 2016-04-26 - v1.4.0

* Merged #24 Add methods for getting issue history - [pilov-pa](https://github.com/pilov-pa)
* Improved XML call for getting issue history and worktimes and some other calls.

### 2016-04-25 - v1.3.0

* Merged #23 Remove dublicated xml declaration - [pilov-pa](https://github.com/pilov-pa)
* Added AgileBoard settings call

### 2016-02-15 - v1.2.4

* Merged #22 Fix error getting login of the author of WorkItem - [stingmu](https://github.com/stingmu)

### 2016-02-14 - v1.2.3

* Merged #19 Fix of create issue method - [angerslave](https://github.com/Angerslave)
* Removed non project related lines from .gitignore

### 2016-02-11 - v1.2.2

* Merged #19 Re-added PHP 5.4 support, Thanks to Angerslave

### 2016-02-08 - v1.2.1

* Just README and CHANGELOG updates

### 2016-02-08 - v1.2.0

* Merged #15 (new methods available) Thanks [@angerslave](https://github.com/Angerslave)

### 2015-12-06 - v1.1.0

* Dropped support for PHP lower than 5.6
* Merged #14
* Merged #13
* Merged #12
* Merged #11
* Merged #10
* Merged #9
* Merged #8
* Merged #7

### 2016-02-08 - v1.0.10

* A lot of new methods added (updateIssue, deleteIssue, createAttachment, importAttachment, importLinks, importIssues, importWorkitems, getWorkitems)
* Merged #7 from REDLINK/fix-createIssue
* Merged #8 from REDLINK/replace-urlencode-with-rawurlencode
* Merged #9 from REDLINK/feature-createAttachment
* Merged #10 from REDLINK/set-mimetype
* Merged #12 from REDLINK/feature-newIssueMethods

### 2015-02-10 - v1.0.9

* Merged #6 'Fetch issues by filter only + with comments'. Thanks [@chabberwock](https://github.com/chabberwock)

### 2015-01-15 - v1.0.8

* Merged #5 'Fixed executing queries.'. Thanks [@wdamien](https://github.com/wdamien)
* Added example for executing simple command

### 2014-12-02 - v1.0.7

* Improved error handling - On 404 error, the call will throw a `YouTrack\NotFoundException`
* Improved error handling - `YouTrack\Exception`/`YouTrack\Error` is now aware of JSON responses
* Improved connection request method. If the body is array it will no longer check if the file exists (Notice was thrown by PHP)

### 2014-11-29 - v1.0.6

* Fixed Issue #4, Improved `getAccessibleProjects`, see `examples/get-all-projects.php`. Thanks [@openWebX](https://github.com/openWebX)

### 2014-11-29 - v1.0.5

* Fixed Issue #3, Added method `getUserRoles`, see `examples/get-user-roles.php`. Thanks [@openWebX](https://github.com/openWebX)
* Improved exception handling (on 403 errors, an `NotAuthorizedException` will be thrown)
* YouTrack-Exceptions are now `YouTrack\Error` aware (`$e->getYouTrackError()`)

### 2014-11-05 - v1.0.4

* Fixed Issue #2, Throw exception `YouTrack\IncorrectLoginException` on incorrect login or password.

### 2014-10-14 - v1.0.3

* Added support for long parameter values for method `createIssue` (It was not possible to do a request with more than 8205 chars (InCloud, nginx 414-Error))
* Improved DocBlocs for Connection class methods

### 2014-09-01 - v1.0.2

* Added more parameters (full support now) for `executeCommand`. Thanks [@1ed](https://github.com/1ed). See [Apply Command to an Issue](http://confluence.jetbrains.com/display/YTD5/Apply+Command+to+an+Issue)

### 2014-09-01 - v1.0.1

* Added executeCountQueries ([Get Number of Issues for Several Queries](http://confluence.jetbrains.com/display/YTD5/Get+Number+of+Issues+for+Several+Queries)). See `./examples/query-count.php`. (Thanks [Limelyte](https://github.com/Limelyte/youtrack/commit/4e4f30e2a118e20f8f364119c37f3e17f38addfa)).
