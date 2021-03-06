pt framework
===========================
*An easy-to-use and portable PHP Framework*


What is pt?
---------------------------
Pt is an easy-to-use and portable PHP framework. It facilitates your development, making it easier and smoother.


Getting Started
---------------------------

##### 1. Copy pt-framework in your project.
Copy `class`,`common`,`conf`,`language` folders and `common.php` into your project's folder.

##### 2. Create folders.
Create `log`, `template` folders in the project (folders' name can be changed in config).<br />
And set `log` folder writeable.

##### 3. Create your first page
And coding this:

```php
// session start
define("SESSION_ON", true);

// define project's config
define("CONFIG", '/conf/web.conf.php');

// debug switch
define("DEBUG", true);

// include framework entrance file
include('./common.php');
```

##### 4. If you want create a **single** entry project, to read [route](https://github.com/page7/pt/wiki/Route) page.
#####    Or not, keep reading [datebase](https://github.com/page7/pt/wiki/Datebase) or [template](https://github.com/page7/pt/wiki/Template) page.


User Guide
---------------------------
View project's [WIKI](https://github.com/page7/pt/wiki)


Change Log
---------------------------
######Alpha 0.1

		Date: 2014-10-06
		Contributor: nolan
		* This is the first version.

######Alpha 0.2

		Date: 2015-04-13
		Contributor: nolan
		* Add namespace "pt\framework" and "pt\tool".
		* Add "pt\framework\debug" class.
		* Add "pt\framework\debug\console" class to print debug message into browser's console.
		* Move function "charset_convert" into class "pt\tool\string".
		* Move function "path_by_str" into class "pt\tool\string", rename "pad_split".
		* Move functions "_is_writable", "_mkdir", "mkdirs" into a new class "pt\tool\file".
		* Remove function "addslashes_deep", "trace".

######Beta 1.0

		Date: 2015-05-26
		Contributor: nolan
		* Add "route".
		* Add Project's wiki.

######Beta 1.1

		Date: 2015-10-15
		Contributor: nolan
		* Add "event", "filter" into framework.
		* Add event's trggiers. Search : "event::trigger" or "filter::apply"
		* UPdate template::$dir to template::$package, and change access for protected.
		* Update class "language" about Gettext not expanded.
		* Remove "template" class's "callback" option.
		* Optimize the filename.
			add path "common\pt", and move config.php and func.php into.
			rename all config file to *.conf.php
		Update Notice:
		* Replace All template::$dir=* to template::package(*).
		* Class "pt\tool\action" and "pt\tool\filter" will be remove for v2.0.
		* Some file path and name be changed, please check.