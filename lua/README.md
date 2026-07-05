# 错字错音提示使用方法简介
## 使用步骤

1. 在你使用的方案文件`*.schema.yaml`中，确保此功能已启用

```yaml
engine:
  filters:
    - lua_filter@corrector      # 错音错字提示，确认此行没有被注释掉
```

2. 从本仓库下载`corrector.lua` 文件
3. 在本地打开`RIMEUserFolder\lua\corrector.lua`
	- 在RIME上右键-用户文件夹即可进入RIMEUserFolder
4. 手工将本仓库中的词条合并到该文件中
