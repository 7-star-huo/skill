---
name: free-tier-tracker
description: >
  免费/低价产品追踪器。追踪腾讯、阿里云、Google、NVIDIA、AWS、Oracle 等大厂的
  免费产品、免费API、免费额度、永久免费层以及 100 元以下的低价体验产品。
  支持按厂商、类别、价格筛选，可用于定期检查新资源、生成白嫖清单、提醒到期时间。
  触发场景：用户提到"免费产品"、"白嫖"、"免费API"、"免费额度"、"免费云平台"、
  "免费试用"、"薅羊毛"、"免费开发者工具"、"check free tier"、"有哪些免费的"等。
agent_created: true
created: 2026-05-21
version: "1.0"
---

# 免费/低价产品追踪器 (Free Tier Tracker)

追踪各大厂商的免费产品、免费API、低价体验产品（100元以下），用于提醒和查找"白嫖"机会。

---

## 核心能力

1. **查询** - 按厂商、类别、价格筛选免费/低价产品
2. **对比** - 同类产品横向对比，帮助选择最佳方案
3. **提醒** - 标记限时活动、试用到期时间
4. **更新** - 通过 WebSearch 搜索各厂商最新免费政策，更新知识库
5. **报告** - 生成结构化的免费资源汇总报告

---

## 知识库：当前免费/低价产品总览

> 数据采集时间：2026年5月
> 数据可能随时变化，建议每次使用时先用 WebSearch 验证关键数据。

---

### 一、🤖 AI/LLM 大模型 API（免费）

| 平台 | 代表模型 | 免费额度 | 有效期 | 申请方式 | 需梯子 |
|------|---------|---------|--------|---------|--------|
| **NVIDIA NIM** | DeepSeek-V4, Llama 4, Qwen 3.5, Mistral Large 3 等 50+ 模型 | 免费积分制，40 RPM，无需信用卡 | 长期 | build.nvidia.com 注册，支持中国手机号验证 | 否 |
| **智谱AI (GLM)** | GLM-4-Flash, GLM-Z1-Flash | **永久免费**，无Token限制（限30并发）；新用户额外送 2000万 Token | 永久 | open.bigmodel.cn 注册 | 否 |
| **硅基流动 (SiliconFlow)** | DeepSeek-R1-0528, Qwen3-8B, GLM-4-9B 等 | 每模型 1000 RPM | 长期 | api.siliconflow.cn 注册 | 否 |
| **ModelScope 魔搭** | DeepSeek-R1, Flux.1, QWen-Image 等 | 每天 2000 次调用（DeepSeek-R1深度版200次/天） | 每日刷新 | modelscope.cn 注册 | 否 |
| **Google AI Studio** | Gemini 2.5 Flash | 30 RPM / 1440 RPD（每天1440次） | 长期 | Google账户登录 aistudio.google.com | 是 |
| **Groq** | Llama 系列 | 每天 1000 次请求，6000 tokens/分钟 | 长期 | groq.com 注册 | 是 |
| **Cloudflare Workers AI** | LLM/嵌入/图像/音频模型 | 每天 10,000 Neurons | 每日刷新 | Cloudflare 账户 | 否 |
| **OpenRouter** | DeepSeek, Kimi, Qwen, Mistral 等 | 每天 50 次免费；充值 $10 解锁 1000 次/天 | 长期 | openrouter.ai 注册 | 否 |
| **GitHub Models** | GPT-4.1-mini, GPT-4.1, GPT-4o | 15 RPM / 150 RPD | 长期 | GitHub 账户直接使用 | 否 |
| **HuggingFace** | 数千开源模型（≤10GB） | 免费推理 API（积分制） | 每月重置 | huggingface.co 注册 | 部分需 |
| **月之暗面 Kimi** | Kimi 系列 | 每分钟 3 次请求，无限Token总量；个人认证送 15 元 | 长期 | platform.moonshot.cn 注册+认证 | 否 |
| **阿里百炼** | Qwen3, DeepSeek, Kimi 系列 | 每模型 100万 Token（新用户） | 3个月/永久 | bailian.console.aliyun.com 申请 | 否 |
| **腾讯混元** | 混元系列 | 100万 Tokens/年 | 1年 | cloud.tencent.com 申请 | 否 |
| **百度千帆** | 文心系列 | 每模型 100万 Tokens/3个月 | 3个月 | cloud.baidu.com 申请 | 否 |
| **讯飞星火** | 星火系列 | 新用户测试额度（含绘图、联网搜索） | 一次性 | xinghuo.xfyun.cn 注册 | 否 |
| **Mistral** | Mistral 系列 | 1 req/s，500K tokens/min | 免费测试中 | console.mistral.ai 注册 | 是 |
| **AI21 Labs** | Jamba Large/Mini | $10 积分（无需信用卡） | 一次性 | ai21.com 注册 | 是 |
| **Fireworks AI** | 多模型 | $1 积分 | 一次性 | fireworks.ai 注册 | 是 |
| **Cohere** | command-a 系列 | 20 RPM | 长期 | api.cohere.ai 注册 | 是 |
| **Cerebras** | 多模型 | 30 RPM，60K tokens/min | 长期 | inference.cerebras.ai 加入等待列表 | 是 |

### 二、🤖 AI/LLM 第三方聚合平台

| 平台 | 代表模型 | 免费额度 | 有效期 | 需梯子 |
|------|---------|---------|--------|--------|
| **ChatAnywhere** | GPT-4o-mini, GPT-5 | 每天每IP 200 次 | 每日重置 | 否 |
| **GemAI** | GPT-5.1, Gemini-3 Pro, Claude Sonnet 4.5, DeepSeek-v3.2, Grok-4 | 注册送 ¥100 | 一次性 | 否 |
| **API520** | Claude-Opus-4.5, Gemini-3 Pro, Kimi-K2 | 注册送 ¥100 | 一次性 | 否 |

---

### 三、🖥️ 云计算平台免费套餐

| 厂商 | 试用金 | 永久免费资源 | 注册难度 | 需信用卡 |
|------|--------|-------------|---------|---------|
| **Oracle Cloud** | $300 / 30天 | ⭐最豪华：4核24GB ARM + 2台 AMD 1GB + 200GB存储 + 10TB流量/月 | ⭐⭐⭐⭐⭐ 极难 | 必须（审核严） |
| **AWS** | $200 / 12个月 | 30+服务：Lambda 100万次/月、S3 5GB、DynamoDB 25GB、CloudFront 1TB | ⭐ 简单 | 必须（$1预扣） |
| **GCP** | $300 / 90天 | 1台 e2-micro (1vCPU/0.6GB) + Cloud Functions/Run 200万次/月 + BigQuery 1TB | ⭐⭐ 较简单 | 必须（可能$10保证金） |
| **Azure** | $200 / 30天 | B系列 VM 750小时/月（前12月） + Functions 100万次 + Cosmos DB 25GB | ⭐⭐ 较简单 | 必须（小额预扣） |
| **阿里云** | 免费试用 160+产品 / 3个月 | 轻量服务器 2核2G 38元/年、2核4G 199元/年 | ⭐ 简单 | 否（需实名） |
| **腾讯云** | Lighthouse 企业版 4核8G/12M/180G SSD（试用） | 个人版 2核2G | ⭐ 简单 | 否（需实名） |
| **华为云** | 新用户免费试用 | 多种产品试用 | ⭐ 简单 | 否（需实名） |
| **移动云** | 1个月 2核4G | - | ⭐ 简单 | 否 |

---

### 四、💰 100元以下低价产品（极具性价比）

| 厂商 | 产品 | 价格 | 说明 |
|------|------|------|------|
| **阿里云** | 轻量服务器 2核2G | **¥38/年** | 新用户专享 |
| **阿里云** | 轻量服务器 2核4G | **¥199/年** | 新用户专享 |
| **腾讯云** | Lighthouse 续费 | **¥38/年起** | 试用后续费优惠价 3.5折 |
| **Oracle Cloud** | 买号（ARM 4核24G） | **约 ¥50** | 绕过注册门槛（注意安全） |
| **DigitalOcean** | 最低 Droplet | **$4/月 (~¥29)** | 512MB/1vCPU/10GB SSD |

---

### 五、🛠️ 免费开发者工具

| 工具 | 免费内容 | 说明 |
|------|---------|------|
| **GitHub** | 无限仓库、Actions 2000分钟/月、Pages 静态托管、Codespaces 60小时/月 | github.com |
| **GitLab** | 无限私有仓库、CI/CD 400分钟/月 | gitlab.com |
| **Cloudflare** | CDN、Pages（无限带宽）、Workers 10万次/天、D1 数据库 5GB、R2 存储 10GB、Tunnel | cloudflare.com |
| **Vercel** | 静态托管、Serverless 100GB带宽/月、1000张图片优化 | vercel.com |
| **Netlify** | 静态托管、100GB带宽/月、300分钟构建 | netlify.com |
| **Supabase** | PostgreSQL 500MB、50MB文件存储、50K月活用户 | supabase.com |
| **MongoDB Atlas** | M0 集群 512MB 存储 | cloud.mongodb.com |
| **PlanetScale** | MySQL 5GB 存储、10亿行读取 | planetscale.com |
| **Firebase** | Spark 免费计划：Auth/DB/Hosting/Functions | firebase.google.com |
| **Neon** | Serverless PostgreSQL 0.5GB存储 | neon.tech |
| **Render** | 静态站点、Web Service 750小时/月 | render.com |
| **Fly.io** | 最多 3 个 VM（256MB 共享CPU）、3GB 持久卷 | fly.io |
| **Railway** | 每月 $5 信用额度 | railway.app |
| **Replit** | 免费在线 IDE、协作编辑 | replit.com |

---

### 六、🌐 免费 CDN / DNS

| 服务 | 免费额度 | 说明 |
|------|---------|------|
| **Cloudflare** | 全球 CDN（不限流量）、DDoS 防护、DNS 解析 | cloudflare.com |
| **jsDelivr** | 免费开源 CDN（npm/GitHub 加速） | jsdelivr.com |
| **unpkg** | npm 包 CDN | unpkg.com |

---

### 七、📦 免费域名

| 服务 | 说明 |
|------|------|
| **Freenom** | .tk/.ml/.ga/.cf 等免费域名（政策不稳定） |
| **EU.org** | 免费 .eu.org 二级域名（审核慢） |
| **Cloudflare** | 域名注册成本价（约 $10/年），无附加费 |
| **GitHub Pages** | username.github.io 免费子域名 |
| **Vercel** | project.vercel.app 免费子域名 |

---

### 八、📧 免费邮件服务

| 服务 | 免费额度 | 说明 |
|------|---------|------|
| **Resend** | 100封/天 | resend.com |
| **SendGrid** | 100封/天 | sendgrid.com |
| **Mailgun** | 试用期 | mailgun.com |
| **Brevo (Sendinblue)** | 300封/天 | brevo.com |
| **Cloudflare** | 邮件路由（转发） | cloudflare.com |

---

### 九、🎓 学生专属福利

| 平台 | 福利 | 条件 |
|------|------|------|
| **GitHub Student Pack** | $200K+ 工具免费（含域名、云服务、IDE 等） | .edu 邮箱验证 |
| **Azure for Students** | $100 信用额度 + 免费服务，无需信用卡 | .edu 邮箱验证 |
| **JetBrains** | 全部 IDE 免费（IntelliJ, PyCharm, CLion 等） | .edu 邮箱验证 |
| **Autodesk** | Fusion 360 等免费 | .edu 邮箱验证 |

---

## 使用方法

### 查询指令示例
- "帮我查一下现在有哪些免费的AI API"
- "AWS 和 GCP 的免费套餐对比"
- "100元以下能买到什么云服务器"
- "NVIDIA 免费 API 怎么申请"
- "有哪些不需要信用卡的免费云服务"

### 更新知识库
当用户要求"检查最新免费资源"或"更新免费产品列表"时：
1. 对每个主要厂商执行 WebSearch，搜索 "[厂商名] [年份] 免费 免费额度 免费套餐"
2. 重点搜索：腾讯云、阿里云、Google Cloud、AWS、Azure、Oracle Cloud、NVIDIA、HuggingFace
3. 对比搜索结果与知识库差异，更新知识库
4. 标注新增、过期、变更的产品

### 生成报告
当用户要求"生成白嫖清单"或"生成免费资源报告"时：
1. 遍历知识库所有分类
2. 按实用程度排序（最推荐排前面）
3. 标注注册难度、是否需要信用卡/梯子
4. 对限时活动加粗提醒
5. 以 Markdown 表格形式输出
6. 附加"本周推荐"板块

---

## 维护规则

### 数据优先级
- **P0 (必须准确)**：免费额度数字、有效期
- **P1 (建议验证)**：申请 URL、注册条件
- **P2 (可能变化)**：模型名称、第三方平台状态

### 过期标记
- 首次采集时记录采集日期
- 大于 30 天的数据建议验证
- 大于 90 天的数据必须标注"[需验证]"
- 明确已失效的产品标记"[已失效]"

### 新增产品标准
符合以下任一条件即可收录：
- 完全免费（无需付费即可获得核心功能）
- 免费试用 ≥ 30 天
- 价格 ≤ ¥100 且为一次性付费
- 免费额度可满足个人开发者日常使用

### 排除标准
- 需要绑定企业资质
- 免费额度零碎无实用价值
- 已停止运营或无维护的平台
- 纯付费产品的"免费咨询"

---

## 注意事项

1. **信息时效性**：厂商政策会随时调整，建议每次关键决策前验证
2. **信用卡风险**：绑定信用卡的平台注意超额风险，及时设置预算告警
3. **科学上网**：部分国际平台需要梯子，知识库中已标注
4. **安全提醒**：不建议购买来路不明的"账号/代注册"服务
5. **合规使用**：仅用于个人学习开发，不用于商业生产环境
