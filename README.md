# Base profile repository

The Base repository is used by the [Jeyzer](https://jeyzer.org) analyzer.\
The Base profile repository is the place holder for the standard shared, master and helper profiles.\
These profiles are compatible with the current Jeyzer project version.


Storage
---------------------------
The Jeyzer base repository is a git repository maintained at :\
https://github.com/jeyzer-repo/base


Shared profile access
---------------------------
The Jeyzer Analyzer is always accessing the latest version of the shared profiles in the base repository.\
https://raw.githubusercontent.com/jeyzer-repo/base/master/shared \
Note that the "master" in this URL is the git branch (not to be confused with a Jeyzer "master" profile).

If you wish to execute the analysis against a constant version, set the desired <version> in the URL specified in the base.xml of your Jeyzer installation : \
https://raw.githubusercontent.com/jeyzer-repo/base/base-<version\>/shared

If you wish to experiment shared profile modifications locally, set the local_first=true in your base.xml and perform the modifications in your local base repository.

As reminder, the base.xml is located in the analyzer/config/repositories directory of your Jeyzer installation.


Master profile access
---------------------------
By default the master profiles are loaded by the Jeyzer Web Analyzer.\
It includes the helper master profiles and the master profiles of open source applications.\
https://github.com/jeyzer-repo/base/master \
https://github.com/jeyzer-repo/base/helper

If you wish to remove the base master profiles from the Jeyzer Web Analyzer, remove the JEYZER_BASE_MASTER_PROFILES_DIR and JEYZER_BASE_HELPER_PROFILES_DIR references from the JEYZER_MASTER_PROFILES_DIR_ROOTS environment variable.\
The JEYZER_MASTER_PROFILES_DIR_ROOTS variable is by default set in the web\apache-tomcat-9.0.73\bin\setenv.bat|sh file of your Jeyzer installation.


Base templates
---------------------------
The template directory contains templates for master and shared profiles.
It contains also a multi-monitor configuration template.


Maintenance and discussions
---------------------------
Feel free to submit new profiles, updates, ideas and suggestions at :\
https://github.com/jeyzer-repo/base/issues \
https://github.com/jeyzer-repo/base/pulls


Profile documentation
---------------------------
https://jeyzer.org/docs/master-profile/ \
https://jeyzer.org/docs/shared-profile/


License
-------

Copyright 2020-2024 Jeyzer.\
Licensed under the [Mozilla Public License, Version 2.0](https://www.mozilla.org/media/MPL/2.0/index.815ca599c9df.txt)
