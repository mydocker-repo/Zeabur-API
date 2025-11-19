# Zeabur-API
zeabur API 操作实例
> 官方文档： https://zeabur.com/docs/zh-CN/developer/public-api
>
> GraphQL API ：https://studio.apollographql.com/public/zeabur/variant/main/explorer

## API密钥
```
#示例token
sk-gx20c4k****qpk4z
```
### 1. 获取可用区域
> 命令
```bash
curl --request POST \
  --url https://api.zeabur.com/graphql \
  --header 'Authorization: Bearer sk-gx20c4k****qpk4z' \
  --header 'Content-Type: application/json' \
  --data '{"query":"query{\n regions {\n name\n id\n}\n}\n"}'
```
> 结果
```json
{
  "data": {
    "regions": [
      {
        "name": "Hong Kong",
        "id": "hkg1"
      },
      {
        "name": "Tokyo, Japan",
        "id": "hnd1"
      },
      {
        "name": "Frankfurt, Germany",
        "id": "fra1"
      },
      {
        "name": "Taipei, Taiwan",
        "id": "tpe0"
      },
      {
        "name": "Taipei, Taiwan",
        "id": "tpe1"
      },
      {
        "name": "Jakarta, Indonesia",
        "id": "cgk1"
      },
      {
        "name": "Silicon Valley, United States",
        "id": "sjc1"
      },
      {
        "name": "California, United States",
        "id": "sfo1"
      },
      {
        "name": "Shanghai, China",
        "id": "sha1"
      }
    ]
  }
}
```
