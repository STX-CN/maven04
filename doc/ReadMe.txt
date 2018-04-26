Maven默认中央仓库

在maven\lib\maven-model-builder-3.5.3.jar中有定义，将其解压
\org\apache\maven\model\pom-4.0.0.xml中，开头几行

  <repositories>

    <repository>
    
  	<id>central</id>

      	<name>Central Repository</name>

	<url>https://repo.maven.apache.org/maven2</url>

      	<layout>default</layout>
   
   	<snapshots>
	
        <enabled>false</enabled>

      	</snapshots>

    </repository>

  </repositories>
定义了默认的中央仓库

设置Maven镜像
在apache-maven-3.5.3\conf\settings.xml中,例如:
  <mirrors>

      <id>maven.net.cn</id>
      <mirrorOf>central</mirrorOf>
      <name>central mirro in china</name>
      <url>http://maven.net.cn/content/groups/public</url>
  </mirror>


阿里巴巴maven中央仓库
<mirror>  
  <id>alimaven</id>  
  <name>aliyun maven</name>  
  <url>http://maven.aliyun.com/nexus/content/groups/public/</url>  
  <mirrorOf>central</mirrorOf>  
</mirror>  


设置Maven本地仓库路径
在apache-maven-3.5.3\conf\settings.xml中
<localRepository>/path/to/local/repo</localRepository>
本地仓库默认路径: usr/.m2/repository