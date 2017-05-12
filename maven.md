### 阿里云镜像  
```  
<mirror>  
  <id>alimaven</id>  
  <name>aliyun maven</name>  
  <url>http://maven.aliyun.com/nexus/content/groups/public/</url>  
  <mirrorOf>central</mirrorOf>   
</mirror>  
```  
### 安装包命令示范  
mvn install:install-file -DgroupId=com.aspose  -DartifactId=aspose-words  -Dversion=15.8.0 -Dpackaging=jar -Dfile=C:\Users\wujunpeng\Desktop\aspose-words-15.8.0-jdk16.jar  
