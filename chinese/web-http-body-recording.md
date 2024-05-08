# 用户隐私-网络请求内容采集

我们认真对待隐私，并理解在拥有足够的信息来解决错误和最终用户隐私之间需要权衡。

我们设计了 SDK，允许开发人员确定要从上报信息中隐藏哪些信息。我们一直在努力改进这些功能，因此，如果您需要我们不支持的隐私功能，请及时告知。

### 采集开关控制

需通过 **控制台** 开启，SDK才会采集网络请求

### 开箱即用的隐私配置

SDK 不会记录包含机密的已知标头,这些标头是：
- `Authorization`
- `Cookie`
- `Proxy-Authorization` 

其余隐私标头可通过API、控制台设置

### Web 隐私控制

| 隐私控制项                                                   | 默认策略               |
| ------------------------------------------------------------ | :--------------------- |
| 网络请求地址白名单                                           | 支持，可通过控制台配置 |
| 网络请求地址黑名单                                           | 支持，可通过控制台配置 |
| 请求白名单，<br />指定地址采集，并且采集指定的`请求头`、`请求体`、`响应头`、`响应体` | 支持，可通过控制台配置 |
| 请求黑名单<br />指定地址采集，并且采集指定的`请求头`、`请求体`、`响应头`、`响应体` | 支持，可通过控制台配置 |
| 按JSONPath采集                                               | 支持，可通过控制台配置 |
