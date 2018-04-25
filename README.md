# fastdfs-test

工程开发参考：[fastdfs-client-java](https://github.com/happyfish100/fastdfs-client-java)
开发、使用commons-pool2连接池封装的工具类
提供简易的上传下载功能.

* FastDFSClient 主要的工具类
* ErrorCode 异常编码
* FastDFSException 异常类
* FileResponseData 文件返回信息
* TrackerServerFactory TrackerServer Factory
* TrackerServerPool TrackerServer Pool

搭好FastDFS环境后
修改config.properties的相关配置，
可直接启动运行项目，通过提供的接口访问，可使用Postman进行测试

# 配置文件配置如下：

# 文件服务器地址
file_server_addr=10.255.255.22:80
# 最大连接数 并发量较大的话可加大该连接数
max_storage_connection=8

## fastdfs为前缀的是FastDFS的配置
fastdfs.connect_timeout_in_seconds=10
fastdfs.network_timeout_in_seconds=30

fastdfs.charset=UTF-8

# token 防盗链功能
fastdfs.http_anti_steal_token=true
# 密钥
fastdfs.http_secret_key=HandFastDFSToken

# TrackerServer port
fastdfs.http_tracker_http_port=80

## Tracker Server, if more than one, separate with ","

fastdfs.tracker_servers=10.255.255.22:22122



# fastdfs-centos安装包：安装环境使用的安装包。
环境：centos。
