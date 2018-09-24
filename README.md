# 配置完整的Solr和Tomcat运行环境

<br/>

# SSM + Solr整合项目

[优雅的实现电商项目中Solr的搜索功能](https://github.com/TyCoding/ssm-redis-solr)
欢迎star

<br/>

# Install

```
git clone https://github.com/TyCoding/solr-tomcat.git
```

<br/>

# Change

If you using git clone project, you neet `solr-tomcat/webapps/solr/WEB-INF/web.xml`，such as:

```
<!-- solrhome的地址，使用自己配置的solrhome的绝对路径 -->
<env-entry>
   <env-entry-name>solr/home</env-entry-name>
   <env-entry-value>/Users/ty/Documents/solr/solrhome</env-entry-value>
   <env-entry-type>java.lang.String</env-entry-type>
</env-entry>
```

<br/>

# Using

If you finish install and change, you can run this solr project, using `./startup.sh` run tomcat, open chrome, input `localhost:8080/solr/index.html` this address. 

If you see this page, it shows that the project is running successfully:

![](peoject.png)

<br/>

# Warning

- 此仓库中提供的tomcat默认使用的8080端口，可能会与你正在启动的项目端口冲突，请自行修改端口。

- 切记修改`tomcat-solr/webapps/solr/WEB-INF/web.xml`，将其中第44行的solrhome地址修改为自己clone的solrhome的地址，不然项目是运行不起来的。
