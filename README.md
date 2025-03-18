# 安装OPA
https://www.openpolicyagent.org/docs/latest/getting-started/#install-opa

# 测试
进入到具体的规则目录下:
opa eval --data policy.rego --input input.json "data"

```json
{
  "result": [
    {
      "expressions": [
        {
          "value": {
            "cloudrec": {
              "d": "aaa",
              "risk": false
            }
          },
          "text": "data",
          "location": {
            "row": 1,
            "col": 1
          }
        }
      ]
    }
  ]
}
```