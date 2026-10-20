# 鲸鱼工具箱 · 总入口

三个产品的统一门户页，一个链接覆盖全部工具。

线上地址：https://lsj666nsyw.github.io/whale-home/

## 文件

只有 `index.html`——单页静态站，无 JS、无依赖、无构建。上传即用。

## 收录的三个产品

| 产品 | 仓库 | 地址 | 定位 |
|---|---|---|---|
| 小工具集 | `whale-tools` | https://lsj666nsyw.github.io/whale-tools/ | 24 个日常小工具，带搜索框 |
| 批量处理三件套 | `whale-batch` | https://lsj666nsyw.github.io/whale-batch/ | 图片/PDF/表格批量操作，最轻最快 |
| 全能办公工具箱 | `office-tools` | https://lsj666nsyw.github.io/office-tools/ | 8 大模块，文档处理最全 |

## 页面结构

1. **Hero 区**：品牌 + 「本地运行、文件不上传、免费」四个信任徽章
2. **产品卡**：3 张，各带功能清单和主色区分（紫=小工具、蓝=批量、绿=办公）
3. **可信度说明**：4 条原则（不上传 / 断网可用 / 不限次 / 手机适配）
4. **FAQ**：5 条，第一条专门解释「三个站有什么区别、该用哪个」
5. **页脚**：3 个产品直链

## 跨站导流

三个产品站各自在 promo 下方有一条 `.crossnav` 导流条，互相链接并指回本门户。
样式定义在各站自己的 CSS 里（类名统一为 `crossnav` / `cn-item` / `cn-home`），
门户页本身不承载导流（它就是导流的目标）。

## 维护注意

- 新增产品：复制一张 `.prod` 卡片，改 `b-blue`/`b-purple`/`b-green` 配色类、
  `.ico` 图标、`<h2>` 标题、功能列表和 `href`，再在 FAQ 和页脚补一处。
- 改产品地址：全局搜 `lsj666nsyw.github.io` 替换，四个仓库都要改
  （门户页 + 三个产品站的 crossnav）。
