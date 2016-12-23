FORMAT: 1A

# API文档
请从修改您自定义的内容。

## 概述
API采用Restful格式，交互的数据格式以json为主。

## 测试接口 [/test]
这是演示用的测试内容。

### 获取内容 [GET]
+ Response 200 (application/json)
      + Attributes (object)
          + id: `e2b8094e-3174-4182-a8b0-99c8a4d3d165` (string, required) - id
          + title: 这是标题 (string, required) - 标题
          + content: 这是内容 (string, required) - 内容
          + updated_at: `2011-09-06T20:39:23Z` (string) - 更新时间
          + created_at: `2011-09-06T20:39:23Z` (string) - 创建时间
