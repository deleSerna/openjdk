# openjdk
work related to openjdk

How to clone a repository

1. Install mercury 
   - follow https://www.mercurial-scm.org/wiki/Download#Mac_OS_X
2. Primarily follow http://openjdk.java.net/guide/repositories.html
   Create and edit the ~/.hgrc file to minimally contain the following entry:

[ui]
username = <openjdk_username>

3. Verify that the ~/.hgrc configuration looks correct. Minimally it should contain the following entries:
$ hg showconfig
ui.username=iris

4. Clone jdk dev repo
   hg clone http://hg.openjdk.java.net/jdk/jdk/
   
   6. http://openjdk.java.net/guide/webrevHelp.html
   7. chmod a+x webrev.ksh
   8. cd jdk
   
   ls
ADDITIONAL_LICENSE_INFO bin                     test
ASSEMBLY_EXCEPTION      configure               webrev
LICENSE                 doc                     webrev.zip
Makefile                make
README                  src
   8. webrev.ksh -m -N -c 8184693
   SCM detected: mercurial

 No outgoing, perhaps you haven't commited.
      Workspace: /Users/nadeeshtv/openjdk/jdk
      Output to: /Users/nadeeshtv/openjdk/jdk/webrev
   Output Files:
	src/java.base/share/classes/java/util/Optional.java
		 patch cdiffs udiffs sdiffs frames old new
     index.html: Done.
Output to: /Users/nadeeshtv/openjdk/jdk/webrev

transfer the web rev http://openjdk.java.net/guide/codeReview.html
scp -r 8184693 ntv@cr.openjdk.java.net:

   
7. http://openjdk.java.net/guide/producingChangeset.html
    
