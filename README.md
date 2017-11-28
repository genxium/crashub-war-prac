# Dependencies

## Gradle 

Please use gradle 2.14.x or up.

## Tomcat 8

- Download a core tarball of Tomcat8 binary from http://mirrors.tuna.tsinghua.edu.cn/apache/tomcat/tomcat-8/v8.5.23/bin/apache-tomcat-8.5.23.tar.gz.
- Untar the downloaded file and name "/path/to/apache-tomcat-8.5.23/" the `${catalina.base}` from now on.

# Building and Running 
- Delete everything under `${catalina.base}/webapps/`.
- proj-root> gradle build
- proj-root> cp -r build/libs/crashub-war-prac.war /path/to/apache-tomcat-8.5.23/webapps/ 
- ${catalina.base}> sh bin/catalina.sh run
- visit `http://localhost:8080/crashub-war-prac/index` in browser.
