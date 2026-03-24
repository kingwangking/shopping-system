# shopping-system

一个用于学习与实践后端开发的项目。当前阶段目标不是完整商城，而是先落地一个最简单订单系统，聚焦：记录、查询、统计。

## 项目定位
- 背景目标：将原有纸质交易记录流程信息化。
- 当前范围：订单记录、订单查询、订单统计。
- 暂不包含：商品、库存、营销、支付闭环等商城能力。

## 文档目录
- [项目背景分析](./docs/背景分析.md)
- [架构设计（初版）](./docs/架构设计.md)
- [架构设计图（初版）](./docs/架构设计图.md)

## 开发环境
- Node.js：建议 20+
- npm：建议 10+
- Chrome：用于 Mermaid CLI 渲染（已通过 `docs/diagrams/puppeteer-config.json` 指定路径）

## 首次安装
```bash
npm install
```

## 常用命令
```bash
# 运行测试（占位脚本）
npm test

# 通用图表渲染命令（通过参数指定输入输出）
npm run diagram -- -i docs/diagrams/clean-architecture.mmd -o docs/diagrams/clean-architecture.svg

# 一次性生成项目当前全部架构图
npm run diagram:all
```

## 图表相关文件
- Mermaid 源文件：`docs/diagrams/*.mmd`
- Puppeteer 配置：`docs/diagrams/puppeteer-config.json`
- 导出图片：`docs/diagrams/*.svg`

## 说明
本仓库使用 npm 本地开发依赖管理工具链；Mermaid CLI 已作为 `devDependencies` 安装，不依赖每次临时下载。
