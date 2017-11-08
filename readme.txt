Jenkins pipeline

=======================

http://localhost:9090/


U:\>mvn -version
Apache Maven 3.0.4 (r1232337; 2012-01-17 14:14:56+0530)
Maven home: C:\dev\tools\apache-maven-3.0.4
Java version: 1.7.0_55, vendor: Oracle Corporation
Java home: C:\dev\tools\Java\jdk1.7.0_55\jre
Default locale: en_US, platform encoding: Cp1252
OS name: "windows 7", version: "6.1", arch: "amd64", family: "wi
U:\>java -version
java version "1.7.0_55"
Java(TM) SE Runtime Environment (build 1.7.0_55-b13)
Java HotSpot(TM) 64-Bit Server VM (build 24.55-b03, mixed mode)

mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

D:\practice\maven_project\my-app>mvn compile
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building my-app 1.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-resources-plugin:2.5:resources (default-resources) @ my-app ---
[debug] execute contextualize
[WARNING] Using platform encoding (Cp1252 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory D:\practice\maven_project\my-app\src\main\resources
[INFO]
[INFO] --- maven-compiler-plugin:2.3.2:compile (default-compile) @ my-app ---
[WARNING] File encoding has not been set, using platform encoding Cp1252, i.e. build is platform dependent!
[INFO] Compiling 1 source file to D:\practice\maven_project\my-app\target\classes
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 3.418s
[INFO] Finished at: Tue Nov 07 13:02:55 IST 2017
[INFO] Final Memory: 9M/154M
[INFO] ------------------------------------------------------------------------
D:\practice\maven_project\my-app>

D:\practice\maven_project\my-app>java -cp target/classes com.mycompany.app.App
Hello World!

D:\practice\maven_project\my-app>



=============================

D:\practice\maven_project\my-app>mvn package
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building my-app 1.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-resources-plugin:2.5:resources (default-resources) @ my-app ---
[debug] execute contextualize
[WARNING] Using platform encoding (Cp1252 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory D:\practice\maven_project\my-app\src\main\resources
[INFO]
[INFO] --- maven-compiler-plugin:2.3.2:compile (default-compile) @ my-app ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:2.5:testResources (default-testResources) @ my-app ---
[debug] execute contextualize
[WARNING] Using platform encoding (Cp1252 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory D:\practice\maven_project\my-app\src\test\resources
[INFO]
[INFO] --- maven-compiler-plugin:2.3.2:testCompile (default-testCompile) @ my-app ---
[WARNING] File encoding has not been set, using platform encoding Cp1252, i.e. build is platform dependent!
[INFO] Compiling 1 source file to D:\practice\maven_project\my-app\target\test-classes
[INFO]
[INFO] --- maven-surefire-plugin:2.10:test (default-test) @ my-app ---
[INFO] Surefire report directory: D:\practice\maven_project\my-app\target\surefire-reports

-------------------------------------------------------
 T E S T S
-------------------------------------------------------
Running com.mycompany.app.AppTest
Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0 sec

Results :

Tests run: 1, Failures: 0, Errors: 0, Skipped: 0

[INFO]
[INFO] --- maven-jar-plugin:2.3.2:jar (default-jar) @ my-app ---
[INFO] Building jar: D:\practice\maven_project\my-app\target\my-app-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 4.370s
[INFO] Finished at: Tue Nov 07 13:06:50 IST 2017
[INFO] Final Memory: 11M/219M
[INFO] ------------------------------------------------------------------------
D:\practice\maven_project\my-app>
================================================


geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project (master)
$ git remote add origin https://github.com/geethasunnap/maven_hello_world.git

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project (master)
$ git push -u origin master
Counting objects: 18, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (7/7), done.
Writing objects: 100% (18/18), 1.82 KiB | 0 bytes/s, done.
Total 18 (delta 0), reused 0 (delta 0)
To https://github.com/geethasunnap/maven_hello_world.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

=============================================


http://localhost:9090/configureTools/

https://github.com/geethasunnap/my_app.git


geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ ls
pom.xml  readme.txt  src/  target/

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git add *
warning: LF will be replaced by CRLF in target/surefire-reports/TEST-com.mycompany.app.AppTest.xml.
The file will have its original line endings in your working directory.
warning: LF will be replaced by CRLF in target/surefire-reports/com.mycompany.app.AppTest.txt.
The file will have its original line endings in your working directory.

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git add .

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git commit -m "first commit"
[master (root-commit) aed30b0] first commit
warning: LF will be replaced by CRLF in target/surefire-reports/TEST-com.mycompany.app.AppTest.xml.
The file will have its original line endings in your working directory.
warning: LF will be replaced by CRLF in target/surefire-reports/com.mycompany.app.AppTest.txt.
The file will have its original line endings in your working directory.
 12 files changed, 306 insertions(+)
 create mode 100644 pom.xml
 create mode 100644 readme.txt
 create mode 100644 src/main/java/com/mycompany/app/App.java
 create mode 100644 src/test/java/com/mycompany/app/AppTest.java
 create mode 100644 target/classes/com/mycompany/app/App.class
 create mode 100644 target/maven-archiver/pom.properties
 create mode 100644 target/my-app-1.0-SNAPSHOT-shaded.jar
 create mode 100644 target/my-app-1.0-SNAPSHOT.jar
 create mode 100644 target/original-my-app-1.0-SNAPSHOT.jar
 create mode 100644 target/surefire-reports/TEST-com.mycompany.app.AppTest.xml
 create mode 100644 target/surefire-reports/com.mycompany.app.AppTest.txt
 create mode 100644 target/test-classes/com/mycompany/app/AppTest.class

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ ll
total 16
-rw-r--r-- 1 geetalakshmi 1049089 1714 Nov  7 13:33 pom.xml
-rw-r--r-- 1 geetalakshmi 1049089 5359 Nov  7 14:49 readme.txt
drwxr-xr-x 1 geetalakshmi 1049089    0 Nov  7 12:53 src/
drwxr-xr-x 1 geetalakshmi 1049089    0 Nov  8 14:17 target/

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ rm -rf target/

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    target/classes/com/mycompany/app/App.class
        deleted:    target/maven-archiver/pom.properties
        deleted:    target/my-app-1.0-SNAPSHOT-shaded.jar
        deleted:    target/my-app-1.0-SNAPSHOT.jar
        deleted:    target/original-my-app-1.0-SNAPSHOT.jar
        deleted:    target/surefire-reports/TEST-com.mycompany.app.AppTest.xml
        deleted:    target/surefire-reports/com.mycompany.app.AppTest.txt
        deleted:    target/test-classes/com/mycompany/app/AppTest.class

no changes added to commit (use "git add" and/or "git commit -a")

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git commit -m "removed target"
On branch master
Changes not staged for commit:
        deleted:    target/classes/com/mycompany/app/App.class
        deleted:    target/maven-archiver/pom.properties
        deleted:    target/my-app-1.0-SNAPSHOT-shaded.jar
        deleted:    target/my-app-1.0-SNAPSHOT.jar
        deleted:    target/original-my-app-1.0-SNAPSHOT.jar
        deleted:    target/surefire-reports/TEST-com.mycompany.app.AppTest.xml
        deleted:    target/surefire-reports/com.mycompany.app.AppTest.txt
        deleted:    target/test-classes/com/mycompany/app/AppTest.class

no changes added to commit

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    target/classes/com/mycompany/app/App.class
        deleted:    target/maven-archiver/pom.properties
        deleted:    target/my-app-1.0-SNAPSHOT-shaded.jar
        deleted:    target/my-app-1.0-SNAPSHOT.jar
        deleted:    target/original-my-app-1.0-SNAPSHOT.jar
        deleted:    target/surefire-reports/TEST-com.mycompany.app.AppTest.xml
        deleted:    target/surefire-reports/com.mycompany.app.AppTest.txt
        deleted:    target/test-classes/com/mycompany/app/AppTest.class

no changes added to commit (use "git add" and/or "git commit -a")

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git add .

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git commit -m "removed target"
[master 7cee823] removed target
 8 files changed, 72 deletions(-)
 delete mode 100644 target/classes/com/mycompany/app/App.class
 delete mode 100644 target/maven-archiver/pom.properties
 delete mode 100644 target/my-app-1.0-SNAPSHOT-shaded.jar
 delete mode 100644 target/my-app-1.0-SNAPSHOT.jar
 delete mode 100644 target/original-my-app-1.0-SNAPSHOT.jar
 delete mode 100644 target/surefire-reports/TEST-com.mycompany.app.AppTest.xml
 delete mode 100644 target/surefire-reports/com.mycompany.app.AppTest.txt
 delete mode 100644 target/test-classes/com/mycompany/app/AppTest.class

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git status
On branch master
nothing to commit, working directory clean

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git remote add origin https://github.com/geethasunnap/my_app.git

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)
$ git push -u origin master
Counting objects: 37, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (18/18), done.
Writing objects: 100% (37/37), 8.53 KiB | 0 bytes/s, done.
Total 37 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/geethasunnap/my_app.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

geetalakshmi@DFG61WQ1 MINGW64 /d/practice/maven_project/my-app (master)






