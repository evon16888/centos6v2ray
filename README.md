# 解决CentOS 6.x 安装V2Ray教程

1、先按官方的代码执行一次，执行后COPY出ID和端口

    bash <(curl -L -s https://install.direct/go.sh)
2、创建一个v2ray文件

    vi /etc/init.d/v2ray
3、把下面的内容COPY进去https://raw.githubusercontent.com/evon16888/centos6v2ray/master/v2ray

4、接下来运行以下命令

    chmod a+x /etc/init.d/v2ray
    chkconfig v2ray on
    service v2ray start
 
5、剩下的就是自行编辑官方文档要求的内容,我也给你准备一个例子吧,具体的还需要你自行去查看官方文档:
配置文件目录

    vi /etc/v2ray/config.json
