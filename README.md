# Memory Fragments Plugin Marketplace

官方插件市场索引仓库。

## 使用方式

1. 在 Memory Fragments 应用中打开「插件市场」页面
2. 添加本仓库地址作为市场源：
   ```
   https://github.com/Nicvank/memory-fragments-plugins-marketplace
   ```
3. 浏览并安装插件

## 添加新插件

Fork 本仓库，在 `marketplace.yaml` 中添加插件条目，然后提交 PR。

### 插件条目格式

```yaml
- name: "your-plugin"           # 唯一标识符
  display_name: "插件显示名"
  description: "插件描述"
  version: "1.0.0"
  author: "作者名"
  type: "tool"                  # tool | visualization | analytics | theme | integration
  license: "MIT"
  icon: "🔧"
  source_type: "github"         # github | embedded
  source_url: "https://github.com/your/plugin-repo"
  tags: ["标签1", "标签2"]
```

### Source Types

- `github`: 插件代码在独立 GitHub 仓库
- `embedded`: 插件代码在本仓库 `plugins/` 目录下

## License

MIT
