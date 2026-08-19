# 🏅 achievement-farm

> 用 GitHub Actions 自动做**真实操作**，解锁 GitHub 上**靠自己就能达成**的成就徽章。

## 自动解锁的成就

| 徽章 | 怎么刷到 | 说明 |
|------|----------|------|
| **Pull Shark** | 自动建分支 → 提 PR → 合并 | 每天合 1 个 PR，累计可升级 tier |
| **YOLO** | 不经审查直接合并 PR | 与 Pull Shark 同一次 PR 顺带拿到 |
| **Quickdraw** | 开 issue 并秒关 | 每天开 + 秒关 1 个 issue |
| **Open Sourcerer** | 多语言仓库贡献 | 仓库内含 10 种语言文件 |

## 自动刷不到的成就（需他人互动）

- **Starstruck**：需要别人给你的仓库 star。
- **Galaxy Brain**：需要别人把你的 Discussion 标记为答案。
- **Pair Extraordinaire**：需要合著提交（另一人 co-author）。
- **Public Sponsor**：需要你赞助别人。

这些无法纯程序触发，得靠真实作品 + 主动分发（参见其他仓库的 README 优化）。

## 工作原理

每天 00:30 北京时间，GitHub Actions 自动运行 `.github/workflows/farm.yml`：

1. 取一个时间戳分支，提交一次，开 PR 并**无审查合并** → Pull Shark + YOLO；
2. 开一个 issue 并立刻以 "not planned" 关闭 → Quickdraw；
3. 全程用个人 PAT 推送，贡献计入 `luisdingww-bit` 账号。

> ⚠️ 娱乐性质：成就徽章对求职/作品集帮助有限，真正加分的是 star 与真实项目。本仓库只是让贡献图与成就墙更热闹。

## License

[MIT](LICENSE)
