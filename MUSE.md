# Muse 每日任务说明：daily-picks

每天做一期「羊毛 + GitHub 精选」，发布到 https://devx-star.github.io/daily-picks/

## 环境

- 登录方式：`ssh muse@213.35.111.147`
- 浏览器：VPS 本机 `http://127.0.0.1:9222` 上**已经在运行**的 Chromium，用 CDP 连接，在里面新开标签页操作。
  不要新启动浏览器，不要用 headless。用完关掉自己开的标签页。
- 仓库：`/home/muse/daily-picks`（已 clone，推送权限只限这个仓库）
- 格式模板：仓库里的 `TEMPLATE.md`

## 每天的步骤

1. `cd ~/daily-picks && git pull --rebase`
2. 用浏览器收集素材（见下方来源）
3. 新建 `_posts/YYYY-MM-DD-daily.md`（日期按北京时间），照 `TEMPLATE.md` 的格式写
4. 检查：front matter 的 `date` 正确、每条都有可点开的官方链接、没有重复往期已收录的项目
5. `git add _posts && git commit -m "daily: YYYY-MM-DD" && git push`
6. 等 1–2 分钟，打开 `https://devx-star.github.io/daily-picks/` 确认新一期已经出现
7. 回报：今天收录了几条羊毛、几个项目，以及发布后的链接

## 内容要求

**🐑 羊毛：3–6 条**
- 只收**免费可领**的：免费额度、免费试用（不需绑卡优先）、限免软件/游戏、开发者福利、教育优惠等
- 每条写清：能领到什么、门槛（是否需信用卡/新用户/特定地区）、截止时间、官方链接
- 链接必须是**官方页面**，不要用别人的推荐/邀请链接
- 自己打开确认过还有效才收录

**⭐ GitHub：5–8 个**
- 有意思、实用、或者新奇的项目，不只是星多。避免连续几天收录同一个项目
- 每个写：仓库链接、语言、星数（今日新增）、一句话是干什么的、一句话为什么值得看

## 参考来源（可以自己扩展）

- GitHub：`github.com/trending`（今日）、`github.com/trending?since=weekly`、Hacker News 的 Show HN
- 羊毛：Epic 每周限免 `store.epicgames.com/zh-CN/free-games`、Steam 限免、
  V2EX 的「免费赠送」等节点、Product Hunt、各大云/AI 厂商的免费额度公告、Reddit r/AppHookup、r/googleplaydeals

## 规矩（必须遵守）

- 这台浏览器**没有登录任何账号**。遇到要登录/注册的页面：跳过，不要注册、不要登录
- 遇到验证码或人机验证：跳过该来源，不要尝试绕过
- 不点任何付款、购买、订阅按钮
- 只能修改 `_posts/` 下的文件。不要改 `_layouts`、`assets`、`_config.yml`、`index.html`
- 内容里不放任何个人信息、邀请码、推荐链接
- 拿不准的信息不写；宁可少收录，也不要编造
