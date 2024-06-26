# 用户隐私-视频录制

我们认真对待隐私，并理解在拥有足够的信息来解决错误和最终用户隐私之间需要权衡。

我们设计了 SDK，允许开发人员确定要从上报信息中隐藏哪些信息。我们一直在努力改进这些功能，因此，如果您需要我们不支持的隐私功能，请及时告知。

## 采集开关控制

Web、内嵌webview、H5等网页内容，需要嵌入 **视图界面采集** SDK插件，并在产品**控制台**打开视图界面采集开关，SDK 才会采集数据。

## 隐私控制机制

视图采集内容，通过混淆、遮罩等方式进行隐私处理，处理过程均在 **终端设备**完成，不会上传到服务器

## Web 隐私控制

| 隐私控制项     | 默认策略                                         |
| -------------- | :----------------------------------------------- |
| 严格模式       | 支持，对文本、图像、输入框内容遮罩混淆、忽略输入 |
| 标准模式       | 支持，默认开启                                   |
| 遮罩密码输入框 | 支持，默认开启                                   |
| 遮罩文本       | 支持，可通过控制台配置                           |
| 遮罩图像       | 支持，可通过控制台配置                           |
| 遮罩dom对象    | 支持，可通过API配置，按class配置， `ty-block`    |
| 忽略输入       | 支持，可通过API配置，按class 配置，`ty-ignore`   |
| canvas 画布    | 不采集                                           |

