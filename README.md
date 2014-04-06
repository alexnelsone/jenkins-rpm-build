jenkins-rpm-build
=================

jenkins build job script to automate creation of RPMs.


The goal of the script was to make RPM creation a little bit easier for a particular company I was doing work for.  The idea is that developers 
or persons who need to build RPM files that could just modify spec files and check those into source control.  This script then parses the SPEC file
headers and uses the information to build out an RPM.  Initially settings were duplicated via Makefiles and multiple spec files.

After the job is run the RPMs are copied out of the RPMS/ and SRPMS/ directories out to the root of the workspace to make them easy to find.


Details on why I created this can be found at:

http://www.nelsone.com/2014/04/auto-generating-rpm-from-spec-file-part1.html<br/>
http://www.nelsone.com/2014/04/auto-generating-rpm-from-spec-file-part2.html
