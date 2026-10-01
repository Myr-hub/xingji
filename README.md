# 星际娱乐游戏源码｜Cocos 前端、C++ 服务端与多款子游戏

星际娱乐是一套包含扑克、麻将、捕鱼等玩法的游戏项目。配套资料覆盖前端场景与脚本、C++ 服务端、网站后台、数据库和编译组件，涉及 Android、iOS 与 H5 平台。

本文围绕游戏界面、工程组成与开发学习展开，配有 25 张界面及目录图片，并附两段独立教学示例。

> 本页用于学习与非现金娱乐项目研究，不涉及现金下注、兑换或操控输赢。图片是原项目界面资料，不代表原程序已经完成非现金改造。

## 目录

- [大厅与登录](#大厅与登录)
- [子游戏](#子游戏)
- [扑克界面](#扑克界面)
- [麻将界面](#麻将界面)
- [捕鱼界面](#捕鱼界面)
- [源码组成](#源码组成)
- [技术栈](#技术栈)
- [代码示例](#代码示例)
- [工程检查](#工程检查)
- [交流反馈](#交流反馈)

## 大厅与登录

项目采用横屏布局，包含两套大厅场景。登录、账号入口、大厅背景和个人信息区分别组织在前端场景中，可以结合场景节点学习界面布局、资源引用和页面切换。

**登录场景工程**

![登录场景工程](images/creator-login.webp)

**大厅场景工程（一）**

![大厅场景工程（一）](images/creator-lobby-a.webp)

**大厅场景工程（二）**

![大厅场景工程（二）](images/creator-lobby-b.webp)

## 子游戏

前端资料标注集成 34 个子游戏。以下列出部分玩法名称，不作为完整清单，也不将不同界面或场次重复计入游戏数量。

| 类别 | 部分玩法 |
| --- | --- |
| 扑克 | 斗地主、跑得快、十三水、德州扑克、二人牛牛 |
| 麻将 | 二人雀神、二人血战 |
| 捕鱼 | 李逵劈鱼、大闹天宫、寻龙夺宝 |

## 扑克界面

扑克部分包含场次选择、对局桌面、换桌、准备及规则说明。德州扑克规则页展示手牌、公共牌和组合牌型；十三水使用分道比较的规则说明；斗地主包含手牌排列、叫牌及倍数说明。

下面的图片用于介绍界面与规则呈现方式，不涉及现金玩法或下注策略。

**德州扑克场次界面**

![德州扑克场次界面](images/poker-room.webp)

**德州扑克牌型说明**

![德州扑克牌型说明](images/poker-rules.webp)

**十三水场次界面**

![十三水场次界面](images/shisanshui-room.webp)

**十三水对局桌面**

![十三水对局桌面](images/shisanshui-table.webp)

**十三水规则说明**

![十三水规则说明](images/shisanshui-rules.webp)

**斗地主对局桌面**

![斗地主对局桌面](images/landlord-table.webp)

**斗地主规则说明**

![斗地主规则说明](images/landlord-rules.webp)

<details>
<summary>展开更多扑克场次与准备界面（3 张）</summary>

**二人牛牛场次界面**

![二人牛牛场次界面](images/cards-room.webp)

**二人牛牛准备界面**

![二人牛牛准备界面](images/cards-ready.webp)

**扑克换桌与准备界面**

![扑克换桌与准备界面](images/cards-table.webp)

</details>

## 麻将界面

麻将部分包含二人雀神与二人血战。场次页面、等待状态、手牌区和规则弹窗分别展示了进入游戏到对局中的界面组织。二人血战的规则页包含牌张范围与牌型说明。

**二人雀神场次界面**

![二人雀神场次界面](images/mahjong-room.webp)

**二人雀神等待界面**

![二人雀神等待界面](images/mahjong-waiting.webp)

**二人血战对局桌面**

![二人血战对局桌面](images/mahjong-table.webp)

**二人血战规则说明**

![二人血战规则说明](images/mahjong-rules.png)

## 捕鱼界面

捕鱼采用海底场景，包含炮台、鱼群、鱼种介绍，以及锁定和自动攻击等操作入口。鱼种介绍按类别展示角色图案与数值，适合研究图鉴列表、场景资源和操作按钮的排布。

**捕鱼海底场景（一）**

![捕鱼海底场景（一）](images/fishing-scene-a.webp)

**捕鱼海底场景（二）**

![捕鱼海底场景（二）](images/fishing-scene-b.webp)

**鱼种介绍（一）**

![鱼种介绍（一）](images/fishing-guide-a.webp)

**鱼种介绍（二）**

![鱼种介绍（二）](images/fishing-guide-b.webp)

## 源码组成

| 模块 | 资料范围 |
| --- | --- |
| 前端 | Cocos 场景、JavaScript 脚本、图片、动画及公共资源 |
| 游戏服务 | C++ 内核、服务程序与子游戏模块 |
| 网站 | ASP.NET 网站、管理后台、数据模型和公共库 |
| 数据 | 游戏服务与网站配套数据库资料 |
| 平台 | Android、iOS、H5 及原生客户端相关资料 |
| 编译组件 | 已编译服务程序、后台、接口和网页客户端文件 |

整体资料按前端、服务端、数据库和网站划分。网站工程中可以进一步区分页面、模型、公共库与服务模块；服务端源码与发布输出也需要分别管理。

**源码资料总目录**

![源码资料总目录](images/01-source-overview.png)

**网站与后台工程目录**

![网站与后台工程目录](images/02-web-project.png)

**服务端发布目录**

![服务端发布目录](images/03-server-components.png)

**配套编译组件目录**

![配套编译组件目录](images/04-compiled-package.png)

## 技术栈

| 部分 | 技术 |
| --- | --- |
| 客户端前端 | Cocos2d-html5、JavaScript、Cocos Creator 工程 |
| 游戏服务端 | C++ 自定义内核 |
| 网站与后台 | ASP.NET、C#，资料标注 Web Forms / MVC |
| 游戏数据库 | SQL Server |
| 网站数据库 | MySQL |
| 服务组织 | 资料描述为分布式服务结构，子游戏可独立部署 |

Cocos Creator 工程截图使用 1.8.2，另有使用 1.9.3 打开查看的记录。具体编译环境和兼容范围应以工程配置、依赖和实际测试为准，不能仅凭能够打开场景判断全部功能可运行。

## 代码示例

以下代码是为本文编写的独立 JavaScript 教学示例，用于说明游戏分类和房间准备流程，**不是原项目源码摘录，也不是可直接替换到原工程中的模块**。它们不依赖 Cocos，可单独运行查看结果。

### 游戏分类

用清单保存游戏名称和类别，将显示内容与界面逻辑分开。这里只列出三项示例，不代表项目的完整游戏配置。

```javascript
const games = [
  { id: "landlord", name: "斗地主", category: "扑克" },
  { id: "mahjong", name: "二人雀神", category: "麻将" },
  { id: "fishing", name: "捕鱼", category: "捕鱼" }
];

function findGames(category, keyword = "") {
  return games.filter(game =>
    (!category || game.category === category) &&
    game.name.includes(keyword.trim())
  );
}

console.log(findGames("麻将"));
// [{ id: "mahjong", name: "二人雀神", category: "麻将" }]
```

### 房间准备

房间可以用“等待、进行中、结束”等状态描述。开始对局前，先检查人数、玩家标识和准备状态。示例只检查房间能否开始，不涉及下注、支付或结果控制。

```javascript
function canStartRound(room) {
  if (!room || room.state !== "waiting") return false;
  if (!Number.isInteger(room.capacity) || room.capacity < 2) return false;
  if (!Array.isArray(room.players)) return false;
  if (room.players.length !== room.capacity) return false;

  const ids = new Set();
  for (const player of room.players) {
    if (!player || typeof player.id !== "string") return false;
    if (!player.id.trim() || player.ready !== true) return false;
    if (ids.has(player.id)) return false;
    ids.add(player.id);
  }
  return true;
}

const room = {
  state: "waiting",
  capacity: 2,
  players: [
    { id: "demo-a", ready: true },
    { id: "demo-b", ready: true }
  ]
};

console.log(canStartRound(room)); // true
```

接入真实多人项目时，这类检查应由服务端再次执行，并在同一受保护的状态更新中完成开局；仅凭客户端按钮状态不足以保证一致性。

## 工程检查

1. 核对编辑器版本、项目依赖与资源路径，先检查场景能否完整打开。
2. 区分客户端、游戏服务、网站和数据库，确认各模块的职责与连接关系。
3. 在隔离的本地测试环境中，逐项检查登录、大厅、准备、对局、结算与重连。
4. 使用测试账号和虚拟数据，不导入真实用户资料、支付配置或生产环境凭证。
5. 对 Android、iOS、H5 分别检查布局、输入方式和资源加载，不将单个平台的结果视为全部平台验证通过。

本文不提供未经验证的部署命令。完整源码、依赖包及运行环境未在本次文章整理中接受全量编译、审计或性能测试，因此不承诺开箱即用、固定部署时间或并发规模。

## 交流反馈

文档勘误与开发学习交流：Telegram [@root4433](https://t.me/root4433)。

本仓库仅用于项目资料说明，不公开完整游戏源码包、数据库备份或部署凭证。图片及相关资料的公开使用须符合权利人的授权要求。

仅供学习与非现金娱乐，禁止用于赌博。
