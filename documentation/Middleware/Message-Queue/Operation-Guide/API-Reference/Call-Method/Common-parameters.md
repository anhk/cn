# 公共参数

## 公共请求头

| 头部字段名 | 字段类型 | 是否必填 | 说明                                                         |
| ---------- | -------- | -------- | ------------------------------------------------------------ |
| accessKey  | string   | Required | 用户申请的accessKey                                          |
| signature  | string   | Required | 使用secretKey对signSource进行**hmac-sha1**加密得到的字符串，签名生成规则在“调用方式-签名算法”章节 |
| dateTime   | string   | Required | 本次http请求发出的UTC时间，格式为ISO-8601:2004。UTC时间又称世界标准时间，比北京慢8小时。ISO-8601:2004要求UTC时间最后加一个大写字母Z， 合并表示时，要在时间前面加一大写字母T。示例：北京时间2018年8月14号上午11点37分00秒，转换后dateTime应设置为 2018-08-14T03:37:00Z |
