# Home Assistant Add-on: Arcadia

这是一个给 Home Assistant OS / Supervisor 使用的 Arcadia 自定义 Add-on 包装仓库目录。

## 说明

这个目录不是 Arcadia 源码本体，而是一个 Home Assistant Add-on 封装。

它直接使用上游镜像：

`supermanito/arcadia`

并将 Home Assistant Add-on 的持久化目录映射到容器内的：

`/arcadia`

从而兼容 Arcadia 所需的目录结构。

## 当前状态

当前版本为最小可用封装，包含：

- `config.yaml`
- `DOCS.md`
- `README.md`

## 已配置内容

- Web 端口：`5678`
- Web UI：`http://[HOST]:[PORT:5678]/`
- 持久化目录：`/arcadia`
- 当前声明架构：`amd64`

## 安装方式

1. 创建一个 GitHub 仓库，例如 `my-ha-addons`
2. 将本目录 `arcadia/` 上传到仓库根目录
3. 在 Home Assistant 的 Add-on Store 中添加你的仓库地址
4. 安装 `Arcadia`
5. 启动后点击 “Open Web UI”
