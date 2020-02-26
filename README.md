https://blog.csdn.net/swpu_ocean/article/details/81436075
当你克隆项目到本地后可使用手机号：19940790216，密码：123456进行登录，也可自行注册并将其修改为最高管理权限。


#本地测试
spring.datasource.url=jdbc:mysql://localhost:3306/myblog?useUnicode=true&characterEncoding=utf-8&useSSL=false
spring.redis.host=localhost
spring.datasource.password=数据库密码
spring.redis.password=redis密码

#上线环境
#spring.datasource.url=jdbc:mysql://服务器ip:3306/myblog?useUnicode=true&characterEncoding=utf-8
#spring.redis.host=服务器ip
#server.ssl.key-store=classpath:1838368_www.zhyocean.cn.pfx
#server.ssl.key-store-password=ssl密码
#server.ssl.keyStoreType=PKCS12
#spring.datasource.password=数据库密码
#spring.redis.password=redis密码

spring.datasource.driverClassName=com.mysql.jdbc.Driver
spring.datasource.username=root

server.port=80
banner.charset=UTF-8
server.tomcat.uri-encoding=UTF-8
spring.http.encoding.charset=UTF-8
spring.http.encoding.enabled=true
spring.http.encoding.force=true
spring.messages.encoding=UTF-8

#pagehelper插件
pagehelper.helper-dialect=mysql
pagehelper.reasonable=true
pagehelper.support-methods-arguments=true
pagehelper.params=count

#打印sql语句
#logging.level.com.zhy.mapper.ArticleLikesMapper=debug

#thymeleaf
spring.thymeleaf.cache=false
spring.thymeleaf.mode=LEGACYHTML5

#redis配置
spring.redis.database=1
spring.redis.port=6379
spring.redis.pool.max-active=8
spring.redis.pool.max-wait=-1
spring.redis.pool.max-idle=8
spring.redis.pool.min-idle=0
spring.redis.timeout=0

#favicon设置
spring.mvc.favicon.enabled=false

#文件上传限制
spring.http.multipart.maxFileSize=10Mb
spring.http.multipart.maxRequestSize=10Mb

#########################Druid连接池的配置信息#################
spring.datasource.type=com.alibaba.druid.pool.DruidDataSource
spring.datasource.druid.initial-size=5
spring.datasource.druid.min-idle=5
spring.datasource.druid.max-active=20
#配置获取连接等待超时的时间
spring.datasource.druid.max-wait=60000
#配置间隔多久才进行一次检测，检测需要关闭的空闲连接，单位是毫秒
spring.datasource.druid.time-between-eviction-runs-millis=60000
#配置一个连接在池中最小生存的时间，单位是毫秒
spring.datasource.druid.min-evictable-idle-time-millis=300000
#检测连接是否有效的sql
spring.datasource.druid.validation-query=SELECT'x'
spring.datasource.druid.test-while-idle=true
spring.datasource.druid.test-on-borrow=false
spring.datasource.druid.test-on-return=false
#PSCacheMysql下建议关闭
spring.datasource.druid.pool-prepared-statements=false
spring.datasource.druid.max-pool-prepared-statement-per-connection-size=-1
#配置监控统计拦截的filters，去掉后监控界面sql无法统计，'wall'用于防火墙
spring.datasource.druid.filters=stat,wall,log4j

#配置WallFilte
#spring.datasource.druid.filter.wall.enabled=true
#spring.datasource.druid.filter.wall.db-type=mysql
#spring.datasource.druid.filter.wall.config.delete-allow=false
#spring.datasource.druid.filter.wall.config.drop-table-allow=false
#spring.datasource.druid.filter.wall.config.create-table-allow=false
#spring.datasource.druid.filter.wall.config.alter-table-allow=false
#spring.datasource.druid.filter.wall.config.truncate-allow=false
