# Muse 每日任务说明：daily-picks

每天做一期「羊毛 · 云电脑 · AI · GitHub 精选」，发布到 https://devx-star.github.io/daily-picks/

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

每期四个栏目，按下面顺序排。**同一条内容只放一个栏目**，按「归属」判断放哪。
某个栏目当天确实没有合格内容，可以少收，但要在栏目里写一句「今天没有值得收录的」，不要硬凑。

**🐑 今日羊毛：3–5 条**
- 归属：游戏、软件、域名、会员、开发者工具、教育优惠等**不属于云和 AI** 的免费福利
- 只收**免费可领**的；免费试用优先收不需绑卡的
- 每条写清：能领到什么、门槛（是否需信用卡/新用户/特定地区）、截止时间、官方链接

**☁️ 云电脑 & 云资源：2–4 条**
- 归属：云电脑/云桌面/云手机、VPS 和云服务器、GPU 算力、对象存储、Serverless 等的**免费额度、试用、赠金、限时活动**
  - 例：甲骨文/AWS/GCP/Azure 免费套餐和赠金变化、阿里云无影/腾讯云等云电脑试用、Colab/Kaggle/Lightning 等免费 GPU、新出现的免费 VPS 或建站平台
- 每条额外写清：**配置**（CPU/内存/显卡/流量）、**免费时长或额度**、**要不要绑卡**、**是否限地区或要实名**
- 有明显坑（到期自动扣费、容易被回收、需要国际信用卡）要在门槛里写出来

**🤖 AI 动态 & 免费额度：3–5 条**
- 归属：AI 相关的新闻和福利：
  - **新发布**：重要的新模型、新产品、大版本更新（一句话说清是什么、比之前强在哪）
  - **免费额度**：AI 工具/API 的免费额度、赠送积分、限时免费（门槛写法同羊毛）
  - **值得一试的新工具**：新出的、普通人也能直接用的 AI 产品
- 只收有官方来源（官方博客、官方公告、产品官网）的，不收传闻和营销号二手消息
- AI 相关的**开源仓库**放到 GitHub 栏目，不放这里

**⭐ GitHub 有趣项目：5–8 个**
- 有意思、实用、或者新奇的项目，不只是星多。避免连续几天收录同一个项目
- 每个写：仓库链接、语言、星数（今日新增）、一句话是干什么的、一句话为什么值得看

**所有栏目通用**
- 链接必须是**官方页面**，不要用别人的推荐/邀请链接
- 自己打开确认过还有效才收录
- 开头那句导读，从四个栏目里挑当天最值得看的两三条来写

## 参考来源（可以自己扩展）

- 羊毛：Epic 每周限免 `store.epicgames.com/zh-CN/free-games`、Steam 限免、V2EX 的「免费赠送」等节点、Product Hunt、Reddit r/AppHookup、r/googleplaydeals
- 云电脑 & 云资源：各云厂商的免费套餐页（`oracle.com/cloud/free`、`aws.amazon.com/free`、`cloud.google.com/free`、`azure.microsoft.com/free`）、阿里云/腾讯云/华为云的活动页、V2EX 的「VPS」「云计算」节点、LowEndTalk、Reddit r/selfhosted
- AI：各大模型厂商官方博客和新闻页（OpenAI、Anthropic、Google DeepMind、Meta AI、DeepSeek、通义千问、智谱、月之暗面等）、Hugging Face 热门、Product Hunt 的 AI 分类、Hacker News 首页
- GitHub：`github.com/trending`（今日）、`github.com/trending?since=weekly`、Hacker News 的 Show HN

## 规矩（必须遵守）

- 这台浏览器**没有登录任何账号**。遇到要登录/注册的页面：跳过，不要注册、不要登录
- 遇到验证码或人机验证：跳过该来源，不要尝试绕过
- 不点任何付款、购买、订阅按钮
- 只能修改 `_posts/` 下的文件。不要改 `_layouts`、`assets`、`_config.yml`、`index.html`
- 内容里不放任何个人信息、邀请码、推荐链接
- 拿不准的信息不写；宁可少收录，也不要编造
