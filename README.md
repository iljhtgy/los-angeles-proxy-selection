# 洛杉矶代理ip怎么选：标着洛杉矶却只给美国出口？静态IP能锁城市吗？多少钱够用？（附 SixtyNet 全套餐价格表）

洛杉矶代理 IP 分三类，价格能差出十倍：按 GB 卖的轮换住宅、按 IP 按月卖的静态住宅/ISP、按 IP 或流量卖的机房 IP。搜这个词最容易踩的坑，是买回来发现出口在美国某个地方，就是不在洛杉矶。

如果你要的是一个固定的、独享的洛杉矶住宅 IP 长期挂着，SixtyNet 走的是另一条路：一台洛杉矶 VPS 配一个 AT&T Mobility 住宅 IP，Residential-STARTER 每月 25 美元，年付 260 美元，2 核 2G、40G NVMe、5TB 流量。代价是 80 和 443 端口被封，代理得自己搭。

> **选购速览**
>
> - 只验证洛杉矶本地搜索结果、比外卖配送费、看广告落地：买按 GB 计费的轮换住宅，从 1GB 档试水
> - 要长期养号、看美区流媒体、固定一个 IP 不换：SixtyNet Residential-STARTER，25 美元/月，年付 260 美元
> - 只想要个美国出口，不关心具体城市：别为“洛杉矶”三个字付溢价
>
> 👉 [查看 SixtyNet 洛杉矶住宅 IP 套餐与当前价格](https://sixtynet.net/aff.php?aff=39)

## SixtyNet 全部套餐与价格

SixtyNet 的产品线要先分清：只有 Residential 系列带住宅 IP，其余是普通洛杉矶 VPS。两条线不要混着看。

**Residential 系列（AT&T Mobility 住宅 IP，官网路径即 at-and-t-mobility-residential）**

| 套餐 | 配置 | 流量 / 端口 | 价格 | 订购 |
| --- | --- | --- | --- | --- |
| Residential-STARTER | 2 核 / 2G RAM / 40G NVMe | 5TB / 2Gbps | $25/月；$260/年（标价 $300） | [选这个](https://sixtynet.net/aff.php?aff=39) |
| Residential-MICRO | 4 核 / 4G RAM / 80G NVMe | 10TB / 4Gbps | $45/月；$460/年（标价 $540） | [选这个](https://sixtynet.net/aff.php?aff=39) |
| Residential-MEDIUM | 8 核 / 8G RAM / 160G NVMe | 20TB / 10Gbps | $85/月；$860/年（标价 $1020） | [选这个](https://sixtynet.net/aff.php?aff=39) |
| Residential-LARGE | 16 核 / 16G RAM / 320G NVMe | 40TB / 10Gbps | $165/月；$1660/年（标价 $1980） | [选这个](https://sixtynet.net/aff.php?aff=39) |

四档都标注同一句限制：**因 IP 风控原因，住宅 IP 产品不开放 80 和 443 端口**。

**其余 VPS 套餐（年付价，官网只挂了年付）**

| 套餐 | 配置 | 流量 / 端口 | 年付价格 | 订购 |
| --- | --- | --- | --- | --- |
| IRVINE-PRO-STARTER | 2 核 / 2G / 40G | 5TB / 2Gbps，AS9929 优化中国 | $350（标价 $420） | [查看](https://sixtynet.net/aff.php?aff=39) |
| IRVINE-PRO-MICRO | 4 核 / 4G / 80G | 10TB / 4Gbps，AS9929 | $550（标价 $660） | [查看](https://sixtynet.net/aff.php?aff=39) |
| LAX-STARTER | 2 核 / 2G / 40G | 5TB / 2Gbps，带 DDoS 防护 | $200（标价 $240） | [查看](https://sixtynet.net/aff.php?aff=39) |
| LAX-MICRO | 4 核 / 4G / 80G | 10TB / 4Gbps | $400（标价 $480） | [查看](https://sixtynet.net/aff.php?aff=39) |
| LAX-MEDIUM | 8 核 / 8G / 160G | 20TB / 10Gbps | $800（标价 $960） | [查看](https://sixtynet.net/aff.php?aff=39) |
| LAX-LARGE | 8 核 / 16G / 320G | 40TB / 10Gbps | $1600（标价 $1920） | [查看](https://sixtynet.net/aff.php?aff=39) |
| LAX-Storage-500G | 4 核 / 4G / 300G+200G RAID10 | 10TB / 10Gbps | $400（标价 $480） | [查看](https://sixtynet.net/aff.php?aff=39) |
| LAX-Storage-1TB | 8 核 / 8G / 700G+300G RAID10 | 15TB / 10Gbps | $700（标价 $840） | [查看](https://sixtynet.net/aff.php?aff=39) |
| Los Angeles China Unicom-Premium | AS9929，BGP 会话，100M 基础网络 | 95 计费，3 倍突发 | $2500（标价 $3000） | [查看](https://sixtynet.net/aff.php?aff=39) |

IRVINE-PRO 那一行要多说一句：官网写明它拒绝所有外部探测和扫描，只有白名单或做了端口转发的设备能连；**这款的退款只退到网站余额**。Residential 系列的页面上没有写退款条款，下单前自己问清楚。

## 先搞清楚你要的是哪种洛杉矶 IP

三种形态的计费逻辑完全不同，选错方向后面怎么调参数都是白费。

**轮换住宅代理**按流量卖，IP 来自真实家庭宽带，可以设置粘性会话，也可以每请求换一个 IP。适合短时间高频次、需要看很多个不同 IP 视角的活。

**静态住宅 / ISP 代理**按 IP 按月卖，一个 IP 归你独占，兼具住宅的可信度和机房的稳定性。适合长期登录、账号绑定。

**机房代理**最便宜，但 IP 注册在主机商名下，风控识别起来最先撞上的就是这类。

SixtyNet 属于第二条线的变体：交付物是整台服务器，住宅 IP 独占，流量按月给，代理协议你自己装。它给你的不是“一个 IP 的使用权”，是“一台机器加一个 IP”。

价格差在哪，用流量算一遍就清楚了。按 GB 卖的住宅代理，1GB 起步两三美元，买 5TB 流量要花到上万美元。SixtyNet 的入门款给 5TB 流量、一个固定住宅 IP，25 美元一个月。差距不在性价比，在 IP 数量：前者你买到的是几十万个可轮换的出口，后者只有一个，换不了。

## 标着洛杉矶，未必落在洛杉矶

这是搜“洛杉矶代理ip”最该先确认的一件事。

Murphy Proxies 在自己的洛杉矶页面上写得很直白：你的出口 IP 来自美国池，不是来自洛杉矶本身；静态 ISP 代理按全国分配，不按城市分配；住宅代理只支持州和 ASN 级定位。ProxyEmpire 的口径类似，静态住宅和数据中心代理只按国家销售，锁不到洛杉矶，想要一个固定的洛杉矶地址只能用轮换住宅或移动代理的粘性会话。Surflare 的表述保守一些：可以选择洛杉矶作为城市，社区和邮编级定位正在陆续开放。

同一个“洛杉矶代理”，实际可能落在四个不同层级上：

1. **国家级**：只保证是美国出口，具体城市随机
2. **城市级**：能指定 Los Angeles 这个目标
3. **街区级**：能指定 Van Nuys、Sherman Oaks 这种具体片区
4. **ZIP 级**：能用邮编把范围再缩小

再往上还有一层运营商或 ASN 定位，做移动端测试的人会在意这个。

下单前值得让客服正面回答一句：这个套餐能不能把出口固定到 Los Angeles 这个城市目标？答不上来或者含糊其辞的，多半就是国家级。

## 洛杉矶市内不是一块铁板

洛杉矶市 469.5 平方英里、15 个市议会选区，范奈斯的一户人家和长滩的一户人家，看到的搜索结果、配送费、广告都不一样。所以“洛杉矶”这个定位在实际使用中经常不够细。

ProxyEmpire 的覆盖能说明这个问题的复杂度：整市之外，圣费尔南多谷有 23 个可单独定位的片区，包括 North Hollywood、Van Nuys、Sherman Oaks、Studio City、Tarzana、Woodland Hills、Canoga Park、Reseda、Northridge、Granada Hills、Chatsworth、Sylmar、Pacoima、Panorama City、Sun Valley、Mission Hills、North Hills、Winnetka、West Hills、Valley Village、Sunland、Tujunga、Porter Ranch。县内其他城市如 Santa Monica、Pasadena、Glendale、Burbank、Torrance、Long Beach 也各自是独立目标。

反过来，**好莱坞、Koreatown、Silver Lake、Echo Park 这些市内街区没有独立定位**，只能用“Los Angeles”加 ZIP 缩小范围。移动端更少，能定位的城市只有 Los Angeles、North Hollywood、Van Nuys、Pacoima、Glendale、Inglewood、Pomona、La Puente 八个。

运营商构成也有讲究。洛杉矶家庭宽带一共 8 个品牌，主要是 Spectrum 和 AT&T，另有 Sonic、Race Communications、Bel Air Internet 这类小型光纤商；Los Nettos、Cogent 这种研究网和骨干网被排除在住宅计数之外。移动端是 AT&T、T-Mobile、Verizon，外加 Boost Mobile。Surflare 还指出一个容易搞错的点：Verizon 并没有在洛杉矶提供 Fios 光纤，只在部分区域有 5G 家庭宽带这种固定无线接入。

这些细节决定了你做本地验证时看到的结果真不真实。用一个 Spectrum 家宽的 IP 去看 DoorDash 的配送费，和用一个机房 IP 去看，结论可能完全不同。

## SixtyNet 这种住宅 IP VPS 适合谁

先把不适合的说清楚。

**80 和 443 端口封了**，官网明写是 IP 风控原因。这意味着你不能拿它直接建站，也不能跑需要标准 HTTP 端口的服务。搭 SOCKS5 或 HTTP 代理走 1080、8080 这类端口没问题，做账号登录、流媒体、数据抓取也没问题。如果你的用途必须占用 80/443，得另配中转或 CDN。

**要自己动手**。SixtyNet 不提供开箱即用的代理订阅，你拿到的是 root 权限的服务器，代理软件、认证、IP 白名单都得自己配。习惯在面板里点两下就拿代理凭证的人，这里会多一道工序。

**没有试用入口**。官网目前看不到试用或按小时计费的选项，最少买一个月。Residential 系列的退款条款页面上也没写，只有 IRVINE-PRO 那两款注明了退到余额。第一次买建议月付，别直接上年付。

适合的场景反而很明确：需要一个**固定不变、独享、不跟别人共用**的美国住宅 IP，而且要挂很久。账号运营最怕的就是 IP 池里今天这个明天那个，或者同池子里有人乱来把整段 IP 搞脏。独享 IP 加整台机器，这个问题不存在。

流量给得也宽。5TB 起步，对登录账号、看流媒体、跑小规模采集这类用途，一个月用不完。这跟按 GB 计费的代理是两种消费心理：那边你每开一个页面都在算钱，这边是包月随便用。

延迟方面 SixtyNet 官网没有公布数据。第三方测评里出现过三网平均 173ms 左右、电信约 163ms 的数字，测的是 Cox 线路那一款，不是本文表格里的 AT&T 系列，只能当量级参考。真要卡延迟，买之前问客服要个测试 IP 自己 ping。

👉 [按需选 SixtyNet 月付住宅 IP 套餐](https://sixtynet.net/aff.php?aff=39)

## 按场景选型

判断标准只有一条：**答案会不会因为地理位置而改变**。会，就锁洛杉矶；不会，美国国家级就够，别多花钱。

| 你要做的事 | 该选什么 |
| --- | --- |
| 查 “dentist near me”“taco truck” 这类本地搜索排名、地图结果 | 轮换住宅，城市或 ZIP 级 |
| 比 DoorDash、Uber Eats、Grubhub 的菜单价和配送费 | 轮换住宅，必须 ZIP 级 |
| 跟 Ticketmaster、SeatGeek 的洛杉矶场次库存和票价 | 轮换住宅 + 粘性会话 |
| 验证投给洛杉矶某片区的广告有没有真的落地 | 轮换住宅，小流量多 IP |
| 在 AT&T、T-Mobile、Verizon 网络下测 App 和移动站 | 移动代理，指定运营商 |
| 跟踪 Zillow、Redfin、Realtor.com 的房源和租金 | 轮换住宅，注意请求节奏 |
| 长期养号、看 Hulu/Disney+/Paramount+ 美区库 | 固定住宅 IP，SixtyNet 这类 |
| 只查全美统一的价格和排名 | 美国国家级或州级，不用锁城市 |

采集类的活不要用固定 IP，一个 IP 高频打同一个站，再干净也会被限。反过来，养号的活不要用轮换池，今天洛杉矶明天芝加哥，账号自己就先露馅了。

## 竞品横向参考

三家主流服务商的公开定价，只列已核验的数字，方便你判断 SixtyNet 的位置。

| 服务商 | 产品形态 | 公开价格 | 关键限制 |
| --- | --- | --- | --- |
| ProxyEmpire | 轮换住宅 | 1GB 按量 $3.50；28GB 档 $2.67/GB 合计 $75；1TB 档 $1.50/GB | 静态住宅与机房仅国家级定位；静态住宅 $3.50/1 个 IP 起；机房 $0.35/GB 起 |
| ProxyEmpire | 移动 | $4.50/GB 起，大套餐低至 $2.00/GB | 含城市与运营商定位；支持 HTTP(S)、SOCKS5、UDP，无并发限制，流量可结转，有 $1.97 试用 |
| Surflare | 机房 IP | $2.9/IP/月 | 静态专属 |
| Surflare | ISP IP | $4.2/IP/月 | 静态专属；社区与邮编级定位陆续开放 |
| Surflare | VPN 共享 IP | $3.8/月 | 共享，非独享 |
| Murphy Proxies | 住宅 | 未在页面标价 | 出口来自美国池，非洛杉矶；仅州和 ASN 级定位 |
| Murphy Proxies | 静态 ISP | 未在页面标价 | 全国分配，不按城市 |

把这些摆在一起看，SixtyNet 的位置很清楚：单看 IP 单价，它比 ProxyEmpire 的静态住宅（$3.50/IP 起）贵得多；但它给的是整台服务器加 5TB 流量，不是裸 IP。如果你只是要一个干净的美国静态住宅 IP、不需要算力，纯 IP 产品更省钱。如果你还需要机器跑东西、要自己控协议、要大流量，打包买更划算。

而如果你要的是几百上千个轮换 IP 做采集，SixtyNet 完全不是这个赛道的产品，别买错。

## 常见问题

**能不能固定一个洛杉矶 IP？**

SixtyNet 的住宅 IP 是独享的，机器在洛杉矶机房，IP 在使用期内不变。至于 IP 归属地显示是否落在洛杉矶市区，官网没有给出城市级定位承诺，下单前建议要一个测试 IP，用 ipinfo 之类查一下再决定。

**静态 IP 能锁城市吗？**

多数服务商不能。ProxyEmpire 明确说静态住宅和数据中心按国家销售，Murphy 的静态 ISP 全国分配。需要“固定的洛杉矶地址”时，行业里常见的替代方案是在轮换住宅或移动代理上开粘性会话。SixtyNet 的做法是给你一台洛杉矶机房的服务器加一个住宅 IP，路径不同，但同样要确认 IP 实际归属。

**流量会不会结转？**

ProxyEmpire 明确写了未用带宽可以结转。SixtyNet 官网没有相关说明，按月计费的 VPS 通常是当月清零。如果你的用量波动大，这一条要单独问客服。

**有并发限制吗？**

ProxyEmpire 明确无并发会话限制。SixtyNet 因为是整台 VPS，并发上限取决于你自己的带宽和机器性能，不存在服务商层面的会话数限制。反过来，一台机器一个 IP，同时跑太多线程容易被目标站限速，这是另一回事。

**合法吗？**

在美国使用代理本身合法。真正决定风险的是用途：要遵守你访问的每个网站的服务条款；处理加州居民个人数据时，还要考虑 CCPA 的要求。

## 下单前最后两步

按你的情况对号入座：

- 只想验证几条洛杉矶本地搜索结果、看看外卖配送费差多少 → 买按 GB 的最小档，1GB 就够试，用完再充
- 要长期养号、看美区流媒体、跑固定业务 → SixtyNet Residential-STARTER，25 美元/月，先月付跑一个月
- 用量大到 5TB 都不够、还要更多算力 → 看 MICRO 或 MEDIUM，年付比月付分别省 80 和 160 美元
- 只需要美国出口、不在乎城市 → 别买洛杉矶，美国国家级定位更便宜

下单前确认两件事：一是你的业务是否依赖 80/443 端口，依赖就得改方案；二是找客服要个测试 IP，查一下实际归属地和流媒体解锁情况，别等付完钱才发现 IP 显示在别的州。

👉 [前往 SixtyNet 选择洛杉矶住宅 IP 套餐](https://sixtynet.net/aff.php?aff=39)
