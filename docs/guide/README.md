# go-cqhttp
使用 [mirai](https://github.com/mamoe/mirai) 以及 [MiraiGo](https://github.com/Mrs4s/MiraiGo) 开发的cqhttp golang原生实现, 并在 [cqhttp 原版](https://github.com/richardchien/coolq-http-api) 的基础上做了部分修改和拓展.
文档暂时可查看 `docs` 目录, 目前还在撰写中.

测试版可前往 [Release](https://github.com/Mrs4s/go-cqhttp/releases) 下载。

## 兼容性

#### 接口
- HTTP API
- 反向HTTP POST
- 正向Websocket
- 反向Websocket

#### 拓展支持
> 拓展API可前往 [文档](docs/cqhttp.md) 查看
- HTTP POST多点上报
- 反向WS多点连接
- 修改群名
- 消息撤回事件
- 解析/发送 回复消息
- 解析/发送 合并转发
- 使用代理请求网络图片

## 关于ISSUE

以下ISSUE会被直接关闭
- 提交BUG不使用Template
- 询问已知问题
- 提问找不到重点
- 重复提问

> 请注意, 开发者并没有义务回复您的问题. 您应该具备基本的提问技巧。

## 性能

在关闭数据库的情况下, 加载25个好友128个群运行24小时后内存使用为10MB左右. 开启数据库后内存使用将根据消息量增加10-20MB, 如果系统内存小于128M建议关闭数据库使用. 