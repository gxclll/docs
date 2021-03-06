# 获取链接

获取链接地址，系统将根据参数计算出对应的链接地址

使用`GET`发起请求，请求地址为`/api/v1/stl/a`

```http
GET /api/v1/stl/a HTTP/1.1
```

## 请求 URI

参数名 | 类型 | 必填 | 说明
------ | ------ | ------ | ------ | ------
siteId | 字符串 | 否 | 站点Id
siteDir | 字符串 | 否 | 站点文件夹
channelId | 字符串 | 否 | 栏目Id
contentId | 字符串 | 否 | 内容Id
channelIndex | 字符串 | 否 | 栏目索引
channelName | 字符串 | 否 | 栏目名称
apiKey | 字符串 | 否 | API 密钥，请参考[身份认证](authentication.md)

`/api/v1/stl/a`的其他参数与`<stl:a>`标签一致。

## 返回

名称 | 类型 | 说明
------ | ------ | ------
200 OK | 字符串 | 链接地址
401 Unauthorized | [Error](/error?id=error) | 认证错误
400 BadRequest | [Error](/error?id=error) | 参数错误

## 示例

### 请求示例

```http
GET /api/v1/stl/a?siteId=1
X-SS-API-KEY: 7cd22002-27a7-4c5d-ba4d-a1c108a20eaf
```

### 返回示例

```json
{
  "value": "/site/index.html"
}
```