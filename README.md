# 一键部署 v2ray 到 heroku  [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

1.部署时配置 v2ray core 的版本、Vmess协议的UUID（"alterId"默认为64）和连接缓存。

2.服务端部署后，应 open app ，显示 Bad Request，表示部署成功。

3.更新 v2ray 版本，修改 app settings-->Config Vars-->VER，程序自动重启，通过view Logs确认。

4.客户端配置 client_config.json, 建议使用 cn_sniproxy+websocket+tls 传输协议。

# 部署配置
![Heroku 配置](https://raw.githubusercontent.com/xlwmin/v2ray-heroku/master/images/heroku.png)
* 1、设置自己的App名称（例：xx123,最终访问地址为 xx123.herokuapp.com）
* 2、设置V2ray服务访问ID（UUID格式），UUID通过[https://www.uuidgenerator.net/](https://www.uuidgenerator.net/) 可获取
* 3、设置部署V2rayCore的版本，版本号可在此[https://github.com/v2ray/v2ray-core/releases](https://github.com/v2ray/v2ray-core/releases)查询

# V2ray 配置
![V2ray 配置](https://raw.githubusercontent.com/xlwmin/v2ray-heroku/master/images/v2ray.png)
# 参考 
https://github.com/v2ray/v2ray-core

https://github.com/onplus/v2hero/
