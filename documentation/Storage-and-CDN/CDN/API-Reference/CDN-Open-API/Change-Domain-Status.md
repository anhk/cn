# **服务状态变更**

## **1. 描述**

服务状态变更包括运行/停止/删除 (changeDomainStatus/{status})

## **2. 请求参数**

| **名称**  | **类型** | **是否必填** | **描述**                                                     |
| --------- | -------- | ------------ | ------------------------------------------------------------ |
| username  | String   | 是           | 京东用户名pin                                                |
| signature | String   | 是           |用户签名，通过md5的方式校验用户的身份信息，保障信息安全。</br>md5=日期+username+秘钥SecretKey; 日期：格式为 yyyymmdd; username：京东用户名pin; 秘钥：双方约定; </br>示例：比如当前日期2016-10-23,用户pin:jcloud_00,用户秘钥SecretKey：e7a31b1c5ea0efa9aa2f29c6559f7d61,那签名为MD5(20161023jcloud_00e7a31b1c5ea0efa9aa2f29c6559f7d61) |
| domain    | String   | 是           | 加速域名                                                     |


## **3. 返回参数**

| **名称** | **描述**                                                  |
| -------- | --------------------------------------------------------- |
| status   | 结果状态，表示接口请求成功与否，成功用0表示，其他表示失败 |
| msg      | 提示信息，如发送任务失败的原因等                          |
| data     | 返回数据                                                  |

 

## **4. 调用示例**

- ### **请求地址**

运行域名：https://opencdn.jcloud.com/api/changeDomainStatus/start

停止域名：https://opencdn.jcloud.com/api/changeDomainStatus/stop

删除域名：https://opencdn.jcloud.com/api/changeDomainStatus/delete （注意：域名删除之前需要先停止域名服务，即先停止域名才可删除域名）

- ### **请求示例**

curl请求示例：

```
 curl -H “Content-type: application/json” -X POST -d ‘{“username”:“test_user”,“signature”:“914a3f412fd9bc1eec14bb5eb104d253”,“domain” :“www.b.com”}’ https://opencdn.jcloud.com/api/changeDomainStatus/start
```

* json格式

```
https://opencdn.jcloud.com/api/changeDomainStatus/start
{
    "username" :"test_user",
    "signature" :"d847267fc702273abf394dd0c3128d64",
    "domain" :"www.b.com"
 }
```

- ### **返回示例**

* json格式

```
{
  "status": 0,
  "msg": "成功",
  "data": "www.a.com"
}
```
