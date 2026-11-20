# 工作区说明

## V2EX 自定义样式发布

- 每次将包含 `v2ex/custom/` 样式改动的提交成功推送到远端后，立即在同一轮回复中提供该次发布的 jsDelivr 链接，不要等用户再问。此规则只规定成功推送后的交付内容，不要求在没有发布请求时主动提交或推送。
- 使用实际推送的 GitHub 仓库、完整提交 SHA 和仓库内文件路径。当前仓库为 `SpiritLing/Temp`，普通 CSS 的格式为 `@import url("https://cdn.jsdelivr.net/gh/SpiritLing/Temp@<完整提交SHA>/v2ex/custom/<文件名>.css");`。不要用分支名替代提交 SHA。
- 分别列出本次改动涉及的普通 CSS：松间 `v2ex-minimal.css`、macOS `v2ex-macos.css`、Windows 11 `v2ex-win11.css`。提示用户在 V2EX 自定义样式中只需复制所用主题的一条，替换旧的 `@import`。若改动了 `v2ex-minimal.user.css`，另给 Stylus 安装链接，不把 UserStyle 当作普通 CSS 导入。
- 发出链接前检查 CDN 是否返回成功且内容是新版本。若推送成功但 CDN 暂未可用，仍可给出固定版本的链接，但须说明尚未验证可用；若推送失败，不要把链接说成已发布。
