##食用说明



1.更改ip

vs2017打开项目，点击"调试->webapplication1属性"，找到最下方"应用URL"，更改为"http://<你的ip>:58546/"

2.生成、运行

____



##原理



**与前端**

controller对应URL，访问 <你的ip>:<端口>/hello时，后台响应并调用HelloController中的Index()方法。该方法的返回值将发送给前端作为response.data。



**与数据库**

通过OracleConnection实体建立连接。

（该方法只是展示连接，实际项目中会使用ORM）