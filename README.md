# aliyun-oss-sign
用于返回阿里云oss服务器签名

## 安装
```
npm install aliyun-oss-sign
```
## 使用
```
import ossSign from 'aliyun-oss-sign'
ossSign({
  accessId: 'your OSSAccessKeyId',
  accessKey: 'your OSSAccessKey',
  // 超时时间 单位：毫秒
  expiration: 300000,
  // 最大上传文件大小 单位：字节(b)
  contentLength: 2097152
})
// 返回
{
  policy: 'policy',
  accessId: 'OSSAccessKeyId',
  signature: 'signature'
}
```
