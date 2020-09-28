# Base profile repository

The Base profile repository is the place holder for the standard shared, master and helper profiles.
These profiles are compatible with the current Jeyzer project version.


Storage
---------------------------
The Jeyzer base repository is a git repository maintained at :
https://github.com/jeyzer-repo/base


Shared profile access
---------------------------
The Jeyzer Analyzer is always accessing the latest version of the shared profiles in the base repository.
https://raw.githubusercontent.com/jeyzer-repo/base/master/shared

If you wish to execute the analysis against a constant version, specify this URL in the base.xml of your Jeyzer installation :
https://raw.githubusercontent.com/jeyzer-repo/base/base-<version>/shared

If you wish to experiment shared profile modifications locally, set the local_first=true in your base.xml and perform the modifications in the local base repository.

As reminder, the base.xml is located in the analyzer/config/repositories directory of your Jeyzer installation.


Master profile access
---------------------------
By default the master profiles are loaded by the Jeyzer Web Analyzer.
It includes the helper master profiles ane the master profiles of open source applications.
https://github.com/jeyzer-repo/base/master
https://github.com/jeyzer-repo/base/helper


Maintenance and discussions
---------------------------
Feel free to submit new profiles, updates, ideas and suggestions at :
https://github.com/jeyzer-repo/base/issues
https://github.com/jeyzer-repo/base/pulls


Profile documentation
---------------------------
https://jeyzer.org/docs/master-profile/
https://jeyzer.org/docs/shared-profile/


License
-------

Copyright 2020 Jeyzer.
Licensed under the [Mozilla Public License, Version 2.0](https://www.mozilla.org/media/MPL/2.0/index.815ca599c9df.txt)