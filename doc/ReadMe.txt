MavenĬ������ֿ�

��maven\lib\maven-model-builder-3.5.3.jar���ж��壬�����ѹ
\org\apache\maven\model\pom-4.0.0.xml�У���ͷ����

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
������Ĭ�ϵ�����ֿ�

����Maven����
��apache-maven-3.5.3\conf\settings.xml��,����:
  <mirrors>

      <id>maven.net.cn</id>
      <mirrorOf>central</mirrorOf>
      <name>central mirro in china</name>
      <url>http://maven.net.cn/content/groups/public</url>
  </mirror>


����Ͱ�maven����ֿ�
<mirror>  
  <id>alimaven</id>  
  <name>aliyun maven</name>  
  <url>http://maven.aliyun.com/nexus/content/groups/public/</url>  
  <mirrorOf>central</mirrorOf>  
</mirror>  


����Maven���زֿ�·��
��apache-maven-3.5.3\conf\settings.xml��
<localRepository>/path/to/local/repo</localRepository>
���زֿ�Ĭ��·��: usr/.m2/repository