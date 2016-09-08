# maven-web

<strong>maven web 建项<strong>
<ol>
<li>new -> project -> Maven Project -> maven-archetype-webapp -> Group Id & Artifact Id -> finish
</li>
<li>修改pom.xml,设置UTF-8和jdk版本，并添加servlet-api-2.5.jar的依赖
</li>
<li>index.jsp报错：Build Path -> Configure Build Path -> Java Build Path -> Libraries -> Add Library -> Server Runtime -> Apache Tomcat v7.0 ->finish
</li>
<li>maven项目规定这些文件夹必须存在：src/main/java, src/main/resources, src/test/java, src/test/resources，若没有，应添加：Java Build Path -> Source -> Add Folder -> Create New Folder -> finish
</li>
<li>Java Build Path中Source下，src/main/java, src/main/resource下的Output folder —> Edit -> Specific output folder -> target/classes 同理 src/test/java, src/test/resources对应为target/test-classes
</li>
<li>将项目转为Dynamic Web Project: Build Path -> Project Facets -> 选三个：Dynamic Web Module(2.3),Java(1.7),JavaScript(1.0) -> ok
</li>
<li>设置部署程序集：Build Path -> Deployment Assembly -> 项目部署路径中，若有test项，应该remove -> ok
</li>
<li>测试，新建controller包，在下面建UserServlet.java，并在src/main/webapp/下建index.jsp和login.jsp,并修改web.xml，完成后放入tomcat启动并在浏览器中测试
</li>
</ol>
