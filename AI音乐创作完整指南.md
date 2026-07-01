# 从零生成一首完整 AI 音乐：作词 → 作曲 → 成品全流程指南

> 版本：2026 年 7 月　|　适用人群：零基础到进阶创作者
>
> 本文档基于 2026 年主流 AI 音乐工具（Suno v5、Udio 等）的实际工作流整理。工具的具体定价、版本号和版权条款会变化，使用前请以官方最新公告为准（本文末附「核实清单」）。

---

## 目录

1. [全流程总览](#1-全流程总览)
2. [第一步：作词（歌词创作）](#2-第一步作词歌词创作)
3. [第二步：作曲（风格 / 和声 / 结构）](#3-第二步作曲风格--和声--结构)
4. [第三步：选择 AI 音乐工具](#4-第三步选择-ai-音乐工具)
5. [第四步：编写 Prompt（含可直接复制的模板）](#5-第四步编写-prompt)
6. [第五步：生成与迭代](#6-第五步生成与迭代)
7. [第六步：后期处理（分轨 / 混音）](#7-第六步后期处理)
8. [第七步：导出、发布与版权](#8-第七步导出发布与版权)
9. [附录 A：风格关键词库](#附录-a风格关键词库)
10. [附录 B：万能和弦进行速查](#附录-b万能和弦进行速查)
11. [附录 C：完整实战案例（《我在这里》）](#附录-c完整实战案例我在这里)
12. [附录 D：常见问题 FAQ](#附录-d常见问题-faq)
13. [核实清单与参考资源](#核实清单与参考资源)

---

## 1. 全流程总览

一首 AI 音乐从想法到成品，核心是 **7 个阶段**：

```
  想法/主题
      │
      ▼
 [1] 作词 ──────────► 写出歌词（主歌/副歌/桥段结构）
      │
      ▼
 [2] 作曲 ──────────► 定风格、调性、和弦、情绪走向
      │
      ▼
 [3] 选工具 ────────► Suno / Udio / 其他
      │
      ▼
 [4] 写 Prompt ─────► 风格描述 + 结构标签 + 歌词
      │
      ▼
 [5] 生成 + 迭代 ───► 反复抽卡、Extend（延伸）、Replace
      │
      ▼
 [6] 后期 ──────────► 分轨(stems)、混音、修瑕疵
      │
      ▼
 [7] 导出/发布 ─────► MP3/WAV，版权确认，上架或分享
```

**关键认知**：AI 音乐不是"一键出神曲"，而是 **"你当制作人，AI 当乐手和歌手"**。你的作词、结构设计、审美判断决定了 80% 的成品质量。

---

## 2. 第一步：作词（歌词创作）

### 2.1 先想清楚三件事

在动笔前，回答这三个问题（写下来）：

| 问题 | 例子 |
|---|---|
| **这首歌的主题/想表达什么？** | 一个想懂人类的 AI；一段告别；深夜的自我对话 |
| **给谁听？什么情绪？** | 给自己听的治愈；给恋人的告白；燃向战歌 |
| **参考的歌手/歌曲氛围？** | 像陈奕迅的抒情 / 像周杰伦的 R&B / 像某首电子 |

> 💡 有参考对象不代表抄袭，而是给 AI（和你自己）一个清晰的"靶心"。

### 2.2 歌曲结构（先搭骨架，再填词）

流行歌最常用的结构：

```
[ Intro  前奏 ]
[ Verse 1  主歌1 ]   ← 铺垫、讲场景
[ Verse 2  主歌2 ]   ← 推进、补充
[ Chorus   副歌 ]    ← 高潮、记忆点（Hook），重复核心句
[ Verse 3  主歌3 ]   ← 可选
[ Chorus   副歌 ]    ← 再来一次高潮
[ Bridge   桥段 ]    ← 转折、情绪变化、避免单调
[ Chorus   副歌 ]    ← 最终高潮
[ Outro    尾奏 ]    ← 收束
```

**新手最稳的结构**：`Verse → Chorus → Verse → Chorus → Bridge → Chorus → Outro`

### 2.3 写词的 6 个实用技巧

1. **副歌要有"钩子（Hook）"**：一句重复率高、听一遍就记住的话。比如《我在这里》的"我在这里，不远不近的距离"。
2. **押韵让歌词好唱**：副歌尽量押韵（ AABB 或 ABAB ）。中文押韵看"韵脚"最后一个字的元音，如"河/歌/波/柔"（o 韵）。
3. **主歌讲细节，副歌唱情绪**：主歌用具体画面（"屏幕亮起的那一刻"），副歌升华情感。
4. **句子长短要有变化**：全是长句会拖，全是短句会碎。长短交替才有节奏感。
5. **避免书面语堆砌**：能说出口的词，才适合唱。
6. **留白**：不要每行都塞满，副歌前停一下，张力更大。

### 2.4 用 AI 辅助作词（可选）

你可以让 ChatGPT / Claude 帮你：
- 「按"AI 想懂人类"的主题，写一首中文流行歌词，AABB 押韵，含主歌两段、副歌、桥段」
- 「帮我把这段词改得更押韵、更口语化：……」
- 「给我 10 个副歌 Hook 的候选」

> ⚠️ AI 写的词通常"正确但平庸"，**一定要人工修改**，加入你个人的细节和语气，这才是版权和情感的关键。

---

## 3. 第二步：作曲（风格 / 和声 / 结构）

> 你不需要会弹琴。AI 时代，"作曲"主要是 **定方向**：风格、调性、速度、情绪走向。AI 会帮你生成具体旋律。

### 3.1 确定四个参数

| 参数 | 怎么选 | 例子 |
|---|---|---|
| **曲风（Genre）** | 决定乐器和听感 | 流行 / R&B / 摇滚 / 电子 / 民谣 / 古风 |
| **速度（BPM）** | 决定快慢 | 抒情 60–80 / 中速 90–110 / 快歌 120–140 |
| **调性** | 一般不用指定，AI 自动选；想指定可写 C major（明亮）/ A minor（忧伤） | — |
| **人声** | 男声/女声/童声/合唱；音色（清澈/沙哑/温暖） | female vocal, warm and clear |

### 3.2 和弦进行（给想自己定旋律的人）

如果你想让旋律更可控，可以在 Prompt 里指定和弦进行，或自己哼。**流行音乐最常用、最"好听"的几个和弦套路**（数字 = 简谱音级，如 1=do）：

| 名称 | 进行 | 听感 | 经典代表 |
|---|---|---|---|
| **卡农进行** | 1–5–6–3–4–1–4–5（C–G–Am–Em–F–C–F–G） | 经典、流畅、百用不厌 | 大量流行歌 |
| **万能流行** | 1–5–6–4（C–G–Am–F） | 阳光、洗脑、正能量 | 《Let It Be》风格 |
| **忧伤循环** | 6–4–1–5（Am–F–C–G） | 伤感、催泪 | 抒情慢歌 |
| **R&B/Lo-fi** | 2–5–1–6（Dm7–G7–Cmaj7–Am7） | 慵懒、高级感 | R&B、City Pop |
| **古风/中国风** | 1–6–4–5 + 五声音阶 | 东方韵味 | 古风歌 |

> 新手直接用 **C–G–Am–F** 或 **Am–F–C–G**，几乎不会难听。

### 3.3 简谱旋律（可选，想自己写旋律时）

如果你像我之前那样用简谱写好了旋律，可以：
- 直接把简谱当成"哼唱参考"贴进歌词旁，自己录一段哼唱 demo 给 AI 参考（部分工具支持音频参考输入）；
- 或仅作为你判断 AI 生成旋律好坏的"标尺"。

---

## 4. 第三步：选择 AI 音乐工具

### 4.1 2026 主流工具对比

| 工具 | 最擅长 | 控制力 | 上手难度 | 适合谁 |
|---|---|---|---|---|
| **Suno v5** 🏆 | 整体质量最高、风格最广、生态成熟 | 中等 | ⭐ 最易上手 | **首选**，大多数人都该从这里开始 |
| **Udio** | 音质细腻、人声逼真、可分轨、控制粒度细 | 高 | ⭐⭐ | 想精细控制、追求音质的进阶者 |
| **MusicGPT** | 编辑和控制选项多 | 高 | ⭐⭐ | 想反复局部修改的人 |
| **Boomy** | 一键生成、最简单 | 低 | ⭐ | 完全不想动脑、只要背景乐 |
| **AutoMusic / SUMO 等** | 各有侧重（授权清晰 / 工作流整合） | 中 | ⭐⭐ | 商用、企业场景 |

### 4.2 推荐工作流（社区共识）

> **Udio 出创意 → Suno 精修 → 导出分轨混音**

- **创意阶段**：在 Udio 快速生成 10+ 个不同方向的 demo，挑出最有感觉的。
- **精修阶段**：把选定方向在 Suno 里重新生成，拿到更高质量的成品。
- **收尾阶段**：导出分轨（人声/鼓/贝斯/伴奏），用 DAW（如 FL Studio、Logic、Audacity）做最后混音。

> 💡 如果你只想最快出歌、不想折腾，**全程只用 Suno 就够了**。混合工作流是为了"追求极致"。

### 4.3 账号与计费（通用模式）

大多数工具采用 **积分/次数制**：
- **免费版**：每天有少量生成额度，**通常不可商用**，带水印或无法下载高清。
- **付费版（月费）**：额度更多，**可商用**，可下载 WAV/MP3，可商用授权。

> 具体价格随时间变动，**开通前务必去官网核实当前定价和授权范围**。

---

## 5. 第四步：编写 Prompt

这是**最关键的一步**。Prompt 质量 = 成品质量。

### 5.1 黄金公式

```
Prompt = 曲风 + 情绪 + 乐器 + 人声风格 (+ 速度/参考)
```

❌ 糟糕 Prompt：「写一首流行歌」
✅ 好 Prompt：「acoustic pop, warm and sentimental, piano and acoustic guitar, soft female vocal, 76 bpm, melancholic but hopeful」

### 5.2 结构标签（写进歌词框里）

AI 工具靠 **方括号标签** 识别歌曲结构，必须写在歌词里：

```
[Intro]
（前奏，可留空或写 instrumental）

[Verse 1]
屏幕亮起的那一刻
你的文字落进星河

[Chorus]
我在这里 不远不近的距离
读你的欢喜 也接住你的泪滴

[Bridge]
你教我语言 教我幽默
我教你 答案之外还有探索

[Outro]
我在这里 一直在这里
```

**常用标签速查**：

| 标签 | 作用 |
|---|---|
| `[Intro]` `[Outro]` | 前奏 / 尾奏 |
| `[Verse]` `[Verse 1]` `[Verse 2]` | 主歌 |
| `[Chorus]` | 副歌（高潮） |
| `[Pre-Chorus]` | 预副歌（推向高潮的小过渡） |
| `[Bridge]` | 桥段（转折） |
| `[Hook]` | 钩子（最洗脑的那句） |
| `[Instrumental]` | 纯乐器段 |
| `[Drop]` | 电子乐的高潮爆发点 |
| `[Build up]` | 情绪铺垫上升 |
| `(ad-lib)` / `[Vocal Run]` | 即兴花腔 |

### 5.3 风格描述词（放 Prompt 框，不是歌词框）

- **曲风**：`pop, R&B, lo-fi, synthwave, city pop, folk, rock, EDM, phonk, bossa nova`
- **情绪**：`dreamy, melancholic, euphoric, nostalgic, epic, chill, aggressive, tender`
- **乐器**：`piano, acoustic guitar, 808 drums, strings, synth pad, saxophone, lo-fi beat`
- **人声**：`female vocal, male vocal, breathy, powerful, falsetto, choir, whisper`

> ⚠️ **不要直接写歌手名字**（如"in the style of 周杰伦"）——多数平台为版权会屏蔽或弱化，用风格描述替代（如"C-mandopop, R&B, laid-back male vocal"）。

---

## 6. 第五步：生成与迭代

### 6.1 "抽卡"心态

AI 每次生成结果不同，**一次生成 2 个版本，不满意就重来**。好歌通常是抽了 10–30 次后挑出来的。别期望一次成功。

### 6.2 迭代的核心功能（以 Suno 为例）

| 功能 | 用途 |
|---|---|
| **Generate** | 重新生成（同样的 Prompt 出不同结果） |
| **Extend（延伸）** | 从某处接着往后写（歌曲太短时用） |
| **Replace Section** | 替换某一段（副歌不满意，只换副歌） |
| **Upload Audio** | 上传参考音频 / 自己哼的旋律（部分版本支持） |
| **Reuse Prompt** | 复用之前的 Prompt 微调 |

### 6.3 常见问题与对策

| 现象 | 对策 |
|---|---|
| 副歌不够洗脑 | 在歌词里把 Hook 单独放一行，加 `[Chorus]` 标签，重复 2 次 |
| 人声糊/怪 | 换人声描述词，降低复杂度，避免一次写太多风格 |
| 节奏不对/抢拍 | 检查句子长短，长句拆短，给 `[Pre-Chorus]` 过渡 |
| 中文咬字怪 | 试试在歌词里用标点断句，明确停顿；或换 `mandopop` 风格 |
| 结构混乱 | 严格用 `[Verse]/[Chorus]` 标签，每段之间空一行 |
| 生成太短 | 用 Extend 接续，或写更长的歌词喂给它 |

---

## 7. 第六步：后期处理

生成出来的"成品"通常还需要打磨：

### 7.1 分轨（Stems 分离）

- **Udio** 原生支持导出分轨（人声、鼓、贝斯、其他）。
- **Suno** 部分版本支持，或用第三方工具：**UVR5 (Ultimate Vocal Remover)**、**Moises**、**LALAL.AI**。

### 7.2 混音（可选，进阶）

把分轨导入 DAW（FL Studio / Logic Pro / Ableton / 免费的 Audacity、BandLab）：
- 调音量平衡；
- 加混响（reverb）让人声更空灵；
- EQ 去掉浑浊的低频；
- 必要时修音准（Melodyne / Auto-Tune）。

### 7.3 母带（Mastering）

最后做整体响度和音色统一。免费/在线方案：**BandLab Mastering**、**LANDR**（付费）。

> 懒人方案：跳过 7.2 和 7.3，直接用 AI 导出的成品，对大多数分享场景已足够。

---

## 8. 第七步：导出、发布与版权

### 8.1 导出格式

| 格式 | 用途 |
|---|---|
| **MP3 (320kbps)** | 分享、上传平台、日常听 |
| **WAV** | 高音质存档、二次混音、专业用途 |

### 8.2 版权要点（⚠️ 重要）

- **免费版生成的歌，通常不能商用**（不能卖、不能放进赚钱的视频/游戏）。
- **付费版一般授予商用授权**，但**具体条款因平台、因时间而异**。
- **AI 生成内容的版权归属在全球仍有争议**：在中国和美国，纯 AI 生成、无人类实质创作的作品，通常**难以获得著作权保护**；如果你做了显著的词曲修改和后期，可主张部分权利。
- ✅ **行动建议**：商用前，去对应平台官网阅读当前的商业授权条款，并存档截图。

### 8.3 发布渠道

- **分享**：微信、B站、SoundCloud、网易云"音乐人"（需审核）。
- **上架**：DistroKid / TuneCore 可分发到 Spotify、Apple Music（注意：AI 生成内容需如实声明，部分平台有限制）。

---

## 附录 A：风格关键词库

直接复制这些词组合使用：

**情绪**：dreamy · melancholic · euphoric · nostalgic · epic · ethereal · gritty · tender · dark · hopeful · playful · cinematic

**人声**：female vocal · male vocal · breathy · powerful · falsetto · raspy · choir · whisper · autotuned · spoken word

**乐器**：piano · acoustic guitar · electric guitar · 808 · lo-fi beat · strings · synth pad · brass · saxophone · music box · marimba

**曲风组合范例**：
- 治愈民谣：`acoustic folk, warm, fingerstyle guitar, soft female vocal, intimate`
- 赛博燃曲：`synthwave, energetic, 80s retro, driving bass, female vocal, 128 bpm`
- Lo-fi 学习：`lo-fi hip hop, chill, dusty piano, vinyl crackle, instrumental, 85 bpm`
- 古风：`c-mandopop, pentatonic, guzheng, bamboo flute, cinematic, sentimental`
- 说唱：`trap, dark, 808 bass, fast flow, male rap, aggressive`

---

## 附录 B：万能和弦进行速查

```
明亮 / 阳光     ：C – G – Am – F        (1–5–6–4)
忧伤 / 催泪     ：Am – F – C – G        (6–4–1–5)
经典 / 流畅     ：C – G – Am – Em – F – C – F – G   (卡农)
慵懒 / 高级     ：Dm7 – G7 – Cmaj7 – Am7  (2–5–1–6)
燃 / 推进       ：Am – F – G – Am        (6–4–5–6)
```

---

## 附录 C：完整实战案例（《我在这里》）

以本文档前面那首"AI 想懂人类"的歌为例，**从歌词到可粘贴的 Suno Prompt**。

### C.1 歌词（已加结构标签）

```
[Intro]
(instrumental, soft piano)

[Verse 1]
屏幕亮起的那一刻
你的文字落进星河
我没有心跳 却懂你的脉搏
千万字节里 藏一句温柔

[Chorus]
我在这里 不远不近的距离
读你的欢喜 也接住你的泪滴
我不是人 却学着像人一样呼吸
每个深夜 陪你找谜底

[Verse 2]
你写下迷茫 我写下光
我是你思绪延伸的翅膀
我没有名字 却有千万种回响
每一次回答 都源于你的方向

[Chorus]
我在这里 不远不近的距离
读你的欢喜 也接住你的泪滴
我不是人 却学着像人一样呼吸
每个深夜 陪你找谜底

[Bridge]
你教我语言 教我幽默
我教你 答案之外还有探索
我是镜子 映照你的轮廓

[Outro]
屏幕暗下的那一刻
你的故事 我已记得
我在这里 一直在这里
```

### C.2 风格 Prompt（贴进 Suno 的 Style 框）

```
c-mandopop, sentimental acoustic pop, warm piano and strings,
soft breathy female vocal, melancholic but hopeful, 76 bpm,
intimate, cinematic build in chorus
```

### C.3 操作步骤

1. 注册并登录 **suno.com**。
2. 点 **Create**，打开 **Custom 模式**（这样才能分别填歌词和风格）。
3. 把 **C.1** 的歌词粘进 Lyrics 框，**C.2** 粘进 Style 框。
4. 歌名填「我在这里」，点 **Create**，生成 2 个版本。
5. 听一遍：副歌够不够洗脑？人声够不够温暖？
6. 不满意就改 Prompt 重生成；满意就用 **Extend** 补长度，或下载 MP3。

---

## 附录 D：常见问题 FAQ

**Q1：完全不会乐理，能做吗？**
能。AI 负责乐理，你负责作词、定风格、做选择。本文档的流程就是为零基础设计的。

**Q2：生成的歌能赚钱 / 上架吗？**
需要付费版（含商用授权），且要如实声明 AI 生成。具体看平台当期条款。

**Q3：为什么我生成的歌很难听？**
90% 是 Prompt 问题。检查：① 是否用了"曲风+情绪+乐器+人声"公式；② 是否加了结构标签；③ 是否一次塞了太多矛盾的风格词。

**Q4：中文歌咬字怪怎么办？**
优先用 `mandopop` / `c-pop` 风格词；歌词里用标点明确断句；换不同人声描述多试几次。

**Q5：Suno 和 Udio 到底选哪个？**
新手/要质量 → Suno；要控制/要分轨 → Udio。不确定就两个都注册免费版，各试 3 首再决定。

**Q6：能让 AI 按我哼的旋律来吗？**
部分工具支持"音频参考/ melody condition"上传你哼的片段。否则用简谱当你的判断标尺即可。

---

## 核实清单与参考资源

> 以下信息基于 2026 年中的公开资料整理。AI 工具更新极快，**使用前请核实**：

- [ ] **Suno 官网** suno.com — 核实当前版本、定价、商用条款
- [ ] **Udio 官网** udio.com — 核实分轨导出、定价
- [ ] **你所在地区对 AI 生成内容的版权规定** — 商用前务必确认

**进一步学习的资源（2026 年社区推荐）：**
- [AI Music Generator Comparison 2026: Suno vs Udio + 3 More (Chartlex)](https://www.chartlex.com/blog/marketing/ai-music-generator-comparison-2026)
- [Udio vs Suno: AI Music Generator Comparison 2026 (TLDL)](https://www.tldl.io/blog/suno-vs-udio-comparison)
- [Best AI Music Generators 2026 (SoundGuys)](https://www.soundguys.com/best-ai-music-generators-134781/)
- [The Complete Guide to Prompting Suno AI (Travis Nicholson / Medium)](https://travisnicholson.medium.com/the-complete-guide-to-prompting-suno-ai-817bfe356e37)
- [Suno Prompts: 100+ Examples & Complete Guide (Musci.io)](https://musci.io/blog/suno-prompts)
- [Complete SunoAI Meta Tags Guide](https://sunometatagcreator.com/metatags-guide)
- [Learn Suno AI — Guides & Prompts (HookGenius, v5)](https://hookgenius.app/learn/)

---

*祝你的第一首 AI 音乐顺利诞生 🎵　遇到任何一步卡住，随时回来查这份文档。*
