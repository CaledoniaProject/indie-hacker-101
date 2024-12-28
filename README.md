### 说明

我花费1个月完成了调研工作，目前全流程都完成了验证，供大家参考。

- [产品开发](#产品开发)
  - [1. 需求搜集](#1-需求搜集)
  - [2. 第三方服务集成](#2-第三方服务集成)
  - [3. 产品推广](#3-产品推广)
  - [4. 用户支付](#4-用户支付)
  - [5. 成本控制](#5-成本控制)
- [公司注册](#公司注册)
  - [1. 美国公司注册](#1-美国公司注册)
  - [2. 美国公司维护](#2-美国公司维护)
  - [3. 提取收益](#3-提取收益)
  - [4. 关于ITIN](#4-关于itin)
  - [5. 其他可选动作](#5-其他可选动作)
- [产品生命周期](#产品生命周期)
  - [SaaS创业流程](#saas创业流程)
  - [过程中技能积累](#过程中技能积累)
- [参考文章](#参考文章)

### 产品开发

#### 1. 需求搜集

1. [Product Hunt](https://www.producthunt.com/)
2. [AlternativeTo](https://alternativeto.net/)
3. [Indie hackers](https://www.indiehackers.com/)
4. [Hacker News](https://news.ycombinator.com/)

#### 2. 第三方服务集成

发邮件

* [Resend，免费版每天100封](https://resend.com/pricing)

用户和身份

* [Clerk，免费版10000个用户](https://clerk.com/pricing)
* [Auth0，免费25000个用户](https://auth0.com/)

部署平台 / 后端服务

* [Vercel，可以集成各家服务，如auth0、pg、redis，小应用免费；注册需要验证手机号](https://vercel.com/)
* [Supabase，类似firebase的开源产品，最好用的是登录功能](https://supabase.com/)

稳定性监控

* [OpenStatus，免费网站状态监控，包括页面展示、故障通知等等](https://www.openstatus.dev/)

页面错误监控，均提供免费版

* [Sentry](https://sentry.io/pricing/)
* [BugSnag](https://www.bugsnag.com/pricing/)
* [InspectLet](https://www.inspectlet.com/plans)

数据分析

* [PostHog](https://posthog.com/pricing)

表单

* [Featurebase，免费需求反馈、Change Log维护网站](https://www.featurebase.app/)
* [Tally，表单服务](https://tally.so/)

文档

* [VitePress - Markdown静态网站生成](https://vitepress.dev/)

#### 3. 产品推广

1. 社交媒体: Facebook、Twitter
2. 产品论坛: Reddit、Discord
3. 自媒体: Youtube、TikTok、Instagram、WikiHow

#### 4. 用户支付

主流支付渠道对比如下

| 供应商                      | 类型 | 公司人数 | 费率                | 客服                           |
| --------------------------- | ---- | -------- | ------------------- | ------------------------------ |
| Lemon Squeezy(被Stripe收购) | MoR  | 8        | 5% + $0.5           | 24小时回复                     |
| FastSpring                  | MoR  | 100+     | 5.9% + $0.95 / 8.9% | 3天起步                        |
| Paddle                      | MoR  | 300+     | 5% + $0.5           | 3天起步                        |
| Stripe                      | PSP | 13000+   | 2.9% + $0.3         | Slack实时，邮件小时级回复      |
| PayPal                      | PSP | 20000+   | 4.4% + $0.3         | 客服答非所问，而且无法切换国家 |

供应商情况说明

1. Lemon Squeezy: 负面消息较多，包括服务不稳定、收费产品突然变成免费、CustomData丢失、非美国地区隐藏的提现费用、技术故障处理不透明。但是审核比较松，因此可以作为备选
   * [Don't trust Lemonsqueezy with your business](https://www.reddit.com/r/SaaS/comments/1b3sf2l/dont_trust_lemonsqueezy_with_your_business/)
   * [Paddle vs. Lemon Squeezy - Experiences](https://www.reddit.com/r/SaaS/comments/13noyxv/paddle_vs_lemon_squeezy_experiences/)
   * [Lemon squeezy's Slack channel is shutting down](https://news.ycombinator.com/item?id=42210504)
2. Paddle: 对应用审核严格且不透明，不会告知审核失败原因
3. FastSpring: 无法直接注册开户，需要对方确认
4. Stripe: Stripe不处理税务，需要自行计算[全球税率](https://docs.stripe.com/billing/taxes/tax-rates )

税务问题

1. [Stripe Tax](https://stripe.com/tax/pricing)
2. [Merchant of Record](https://fastspring.com/blog/what-is-a-merchant-of-record-and-why-you-should-care/) 是什么？

注意事项

1. 一定要先提交申请，再去集成支付渠道，否则可能白忙活
2. 条件允许最好接多个渠道，否则用户有投诉的时候可能会被暂停收款，造成业务有损

#### 5. 成本控制

免费云服务器

1. Google/AWS/Azure都可以申请免费服务器，但是一般都有时间限制
2. 微软会提供OpenAI的费用，AI开发者应该先考虑微软云

### 公司注册

#### 1. 美国公司注册

中国大陆身份无法用于开通支付渠道，因此必须注册境外公司。

| 供应商      | 初始费用 | 续费价格 | 初始服务                                             | 州 |
|:------------- |:----------- |:---------------- |:------------------------------------------------------------ |:----- |
| Stripe Atlas  | $500        | $100             | RA + 注册公司 + EIN + 年报 + Stripe + Mercury | DE    |
| Firstbase     | $399        | $149             | RA + 注册公司 + EIN + 年报 + Mercury          | DE/WY |
| WyomingAgents | $154        | $25              | RA + 注册公司 + 年报 + 收费邮箱           | WY    |

手工注册流程

1. 准备护照、专用邮箱、专用手机号、地址证明。无需身份证。
2. 选择一家Register Agent注册公司 (美国公民或者永居才能是RA)。
2. 申请EIN。有SSN在线申请，否则[通过传真提交SS4表格申请](https://www.llcuniversity.com/irs/how-to-apply-for-ein-without-ssn/#form-ss4)，1天搞定。[Fivver链接，需要选$15的，EIN + 147-C](https://www.fiverr.com/search/gigs?query=EIN)，加上手续费$18。
3. 有EIN后，30天内[在线提交BOI](https://boiefiling.fincen.gov/)，流程可以参考[BOI报告申报](https://qinyang.wang/beneficial-ownership-information-report)。
4. 开通企业银行: [Mercury](https://mercury.com/pricing)、[Wise](https://wise.com/us/pricing/)，1天搞定
5. 开通Stripe、关联Mercury银行，10分钟搞定

企业银行选择

1. Mercury，没有限制，存款超过500K可以买美债
2. Brex，门槛很高，不适合初创公司
3. Found、RelayFi，需要美国物理地址才能申请，RA属于虚拟地址

公司起名

1. 可以通过ChatGPT生成，如果实在想不到名字可以考虑以Studio/Lab/Works结尾
2. 注册前先在Google、域名注册商、商标局、州查询是否有重复的情况
3. WY州在[这里查询](https://wyobiz.wyo.gov/Business/FilingSearch.aspx)
4. 美国商标在[这里查询](https://www-search.uspto.gov/)

其他从供应商询问到的信息

1. Mercury: 
   * 不能存款(Stripe提现可以)
   * 美元全球汇款无手续费，可以给中国、香港汇款
   * 可以只要虚拟卡(否则需要通过Register Agent转发，承担快递费用或者丢卡风险)
2. wyomingagents
   * 续费价格费用构成: $100 filling fee + $63 state fee + $25 register agent
   * 邮件扫描费用说明: 超过限制后每封$15，无法决定哪些邮件会被扫描，但是他们会丢弃垃圾邮件，并且州或者联邦政府发送的邮件免费扫描上传
   * 提交BOI $25，申请EIN $250，价格不合理
3. Firstbase优惠码 PARTNER10、LIGHT10、AUTOPILOT10、MAILROOM10
4. EIN: 首次申请EIN，没有SSN不会立即给你CP-575表单，只会平邮到公司注册地址，大概2~3周；147-C可以通过电话申请，会立即传真给你

#### 2. 美国公司维护

合规事项

1. 每年传真提交 Form 1120 + 5472，截止时间4.15、与公司财年无关；Fivver价格$50起步
   1. IRS [Form 1120 退税表](https://www.irs.gov/pub/irs-pdf/f1120.pdf)、[Form 5472 外国人持股表](https://www.irs.gov/pub/irs-pdf/f5472.pdf)
   2. [How Much Does an LLC Cost by State (2024 Guide) - Do LLCs pay taxes?](https://www.llcuniversity.com/llc-filing-fees-by-state/#do-llcs-pay-taxes)
   3. [美国公司LLC如何完成Form1120、Form5472申报](https://zhuanlan.zhihu.com/p/687221777)
   4. 在[NAICS](https://www.naics.com/search/)上查询Business Code，用于填表
   5. [Fivver链接](https://www.fiverr.com/chkhizaraslam/provide-you-the-services-of-tax)，$72、2天搞定，需要提前沟通，未验证。
2. 每年在线提交 State Annual Report，就是给州交钱，价格跟公司净资产有关系，最低$60。最晚提交时间是公司注册月份的第1天，最早可以提前1年提交。
   1. https://www.llcuniversity.com/wyoming-llc/annual-report/
   2. https://wyobiz.wyo.gov/Business/AnnualReport.aspx

美国公司注意事项

1. LLC报税穿透到个人，但报税只需要EIN，并不需要ITIN。有ITIN可以用来申请信用卡，没有只能申请押金卡
2. 有融资需求需要选Corporation，[报税需要提交 Form 1120](https://www.zhihu.com/collection/774430862)

#### 3. 提取收益

根据类型选择[不同的提现方式](https://finally.com/blog/accounting/owners-draw/)，

| 类型 | 所有者提现 | 工资             |
| --------------- | ------------ | ------------------ |
| Sole Proprietor | Yes          | Optional           |
| Partnership     | Yes          | Optional           |
| LLC             | Yes          | Optional           |
| S Corporation   | Yes          | Required (if paid) |
| C Corporation   | No           | Required           |

税务合规

1. 在美国，外国人只要正常提交IRS表格，收益可以离开美国
2. 在中国，类型选择境外/股利收入，每年3~6月自行申报即可

#### 4. 关于ITIN

外国人没有SSN，可以通过IRS申请ITIN用于个人报税。如果只是注册Single Member LLC没有申请的必要，因为此类LLC报税可以通过EIN发起。不过，如果需要在美国申请信用卡则必须有ITIN，否则只能申请押金信用卡。

ITIN申请方法

1. [Fiverr CAA申请大约$260](https://www.fiverr.com/caaitin_com/apply-itin-number-for-your-as-irs-caa)
2. 邮寄护照原件方案丢失概率高
3. 美国大使馆公正护照$50，邮寄费用未知

#### 5. 其他可选动作

准备专用电话号码

1. 美国可以买UltraMobile PayGo，可以京东买，可以转eSIM
2. 英国可以买giffgaff，可以官网买
3. 其他的只能买到流量卡，可以找国外代购
4. **国内小号不支持跟境外号码通信**，不要买

### 产品生命周期

#### SaaS创业流程

1. 找点子，解决用户的需求
2. 快速上线、对接支付，检验产品价值
3. 运营推广
4. 卖给大公司

#### 过程中技能积累

1. 低成本产品开发，如用户界面、后端服务、数据统计、稳定性和错误监控、SEO优化、文档服务
2. 产品运营能力，如运营文案、广告投放、社区维护
3. 业务分析能力，如市场分析、产品定价、成本核算

### 参考文章

基础准备

1. [硬地骇客](https://book.hardhacker.com/toc)
2. [历时两周把海外公司、银行账户、Stripe 都注册下来了，无论收美元还是 USDT，从此实现全球收款国内到账](https://m.okjike.com/originalPosts/64d4e94e58c9056cf4fed028?s=eyJ1IjoiNjJhYTljZTI2N2YwNTAwMDExNDYwOTE5IiwiZCI6Mn0%3D)
3. [AppStore开发者银行账户美国报税表怎么填？协议、税务和银行如何设置？](https://blog.zhheo.com/p/137a3891.html)
4. [《独立开发者的艺术》打造最全的独立开发者指南，一人公司](https://github.com/hua1995116/indiehackers-steps)

获取用户

* [1000UserGuide：对独立开发者和创业者来说，找到前1000个早期用户太关键了。这里精心整理了300多个国内外渠道，适合独立开发者和创业者推广产品的渠道](https://github.com/naxiaoduo/1000UserGuide)
* [如何获取用户](https://sideproject.guide/getting-users)
