# ws-server
websocket server 下载

# 功能介绍   
  用于消息的推送，在最小的资源占用下，提供极限级性能。
# 接口说明
  可自定义认证接口，请参考配置文件内容
  监听是，可以传入jwt，用于身份认证。   
  jwt的解析由config.toml中配置的接口进行解析。需要返回用户的id
  

# 运行   
  需要openssl的支持。   
  在debian下可以直接运行，其它环境下，最好用rust docker   
  运行前，请输入激活码。

# 测试服务器   
  ## 发送测试
  ws://<user>:<password>@host:port/dispatch   
  e.g: ws://root:password@127.0.0.1:9999/dispatch
  发送端只能发送
  ## 接收端，只用于接收
  ws://<id>@host:port/ws   
  e.g:ws://11@host:9999/ws
  

