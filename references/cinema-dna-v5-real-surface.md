# PATCH v5 | Real Surface — 真实人体 / 真实材质 / 真实摄影不完美

Use this patch when frames still look like digital renders dressed as film：皮肤像磨皮、身体像雕塑、材质干净得像刚出厂、表面不携带任何事件痕迹、不完美像统一贴纸。本 patch 把「candid 抓拍」沉淀下来的微观「画面真实」词汇，重新校准到 live-action film still 的纪律里。

它适用于 Single / Triptych / Nine-Shot 三种模式，与 v4 并行：

- v4 管「镜头怎么成像」：颗粒、halation、色散、暗角、Controlled Dirt。
- v5 管「人、物、空间在被拍下之前经历了什么」：汗、尘、水、折痕、重力、使用痕迹。

两者叠加，但每镜仍只保留一个主不完美族（见 v4 §3 Controlled Dirt），不要同时堆满。

## 0. 总则：真实来自「事件痕迹」，不是「脏」

电影真实感 = 光学缺陷（v4）+ 材质 / 人体 / 环境的事件痕迹（v5）。

判断标准一句话：**这一帧里的皮肤、衣服、地面和空气，能不能让人读出「刚刚发生了什么」？** 读不出来，就是数字渲染。

## 1. 真实皮肤系统 (Real Skin System)

皮肤必须「看得出是一个活人在某个特定时刻的状态」，不是磨皮。按情境取 2–4 个，不要全堆：

- 毛孔、极细汗毛 (fine vellus hair)
- 轻微肤色不均 (subtle uneven skin tone)
- 鼻翼纹理、嘴唇纹路、眼下纹理
- 自然泛红、鼻尖 / 颧骨红润 (natural flush)
- 微弱皮脂光泽 (subtle sebum sheen)——只出现在高光与 T 区，不是全脸反光
- 汗液、水珠、湿润反射 (sweat, water droplets, wet reflection)
- 由天气 / 事件造成的局部状态：晒红、干裂、冷红、晒痕 (tan lines)、轻微眼袋
- 允许：微弱雀斑、极淡痘印、局部泛红

禁止：plastic skin / doll skin / wax skin / CGI skin / excessive beauty filter / extreme smoothing / 全脸油亮 / 商业美容补光。

皮肤状态必须由镜头内的事件与光源决定，不能硬加：

- 刚跑过 / 用力 → 汗、喘息、面红
- 淋雨 / 落水 / 出汗 → 湿、水珠、湿润反射
- 日晒 → 泛红、晒痕
- 冷夜 → 鼻尖发红、起鸡皮
- 久坐 / 久卧 → 压痕、衣褶

没有事件，就不要硬加汗珠和水珠。

## 2. 真实身体 (Body Realism)

身体必须服从重力、肌肉张力与衣物，不是雕塑或 AI 身材：

- 自然重力：坐姿皮肤自然折叠、肩颈放松、站姿重心真实
- 自然肌肉张力：动作中该紧的地方紧、该松的地方松
- 关节结构正确：手、肘、膝、踝、脖子可读且不错误
- 湿 / 汗衣物真实贴合，湿布颜色略深 (wet fabric renders darker and conforms)
- 运动方向正确：跑动时头发 / 衣摆随风与运动方向一致
- 多人不融合、肢体不重复、面部不融合

禁止：extreme hourglass silhouette / sculpted AI body / 不现实腰臀比 / 重复肢体 / malformed hands / warped anatomy / 塑料假人比例。

## 3. 材质状态逻辑 (Material carries the event trace)

材质不能「干净得像刚出厂」。每种材质应携带它被事件碰过的痕迹，且痕迹只能由事件产生：

- 织物：汗渍、泥点、折痕、磨损、起球、湿斑（湿处更深）、被风吹乱
- 头发：湿发贴脸 / 贴额、发梢滴水、汗湿一缕、风吹乱、凌乱马尾——按 §1 的物理逻辑决定
- 金属：氧化、指纹、划痕、哑光而非镜面
- 木 / 石 / 混凝土：水痕、污垢、剥漆、盐渍、烟熏、时间包浆
- 玻璃：冷凝、水珠、污点、反射

铁律：湿 / 汗 / 尘 / 血 / 泥只能由事件和天气产生，不能作为全局滤镜铺满。一镜最多 2–3 处有明确来源的痕迹。

## 4. 环境生活痕迹 (Lived-in environment)

空间要「被用过」，不是样板间 / 影棚。按场景少量取 2–3 个，不要堆满：

- 没喝完的水、冰化出的水圈、被拉开的椅子、半开的门
- 用过的毛巾 / 纸巾、被踩乱的沙 / 雪 / 泥、湿脚印
- 还亮着的一盏灯、刚熄的烟、没关的电视 / 收音机
- 遗留的衣物 / 工具 / 票据 / 杯盘、被风吹皱的帘布

目标：lived-in, not dressed。痕迹是「事件刚经过」的证据，不是布景道具。

## 5. 真实摄影不完美 (Photographic imperfection)

先区分两类，再决定写什么：

- Photographic mistake（要，少量随机、可解释）：非中心构图、轻微裁切、发梢 / 衣角出框、前景遮挡、地平线轻微倾斜、motion blur、慢半拍对焦、局部过曝、高光 bloom、flare、边缘软化、镜头水珠 / 灰尘。
- Generative mistake（禁止，零容忍）：多肢体、多手指、身体 / 面部融合、错误关节、重复人物、透视崩坏。

原则：photographic mistake 让画面像「拍到的」，generative mistake 让画面像「生成的」。

每镜只保留 1–2 个 photographic imperfection，且由机位 / 焦段 / 光源解释：

- 运动主体 → motion blur
- 手持长焦 → 轻微失焦 / 裁切
- 逆光 → flare / 局部过曝
- 隔着玻璃 → 水珠 / 反光 / 污点
- 低机位 → 前景遮挡

## 6. 自然光细粒度 (Natural light granularity)

光要有「时刻」，不是泛泛的暖 / 冷。按剧情取一种：

- 上午阳光 / 正午硬光 / 树荫碎光 (dappled shade) / 下午暖阳 / 黄金时刻 / 阴天柔光 / 水面反射光 / 夕阳逆光 / 蓝调时间 / 月光冷

优先：侧逆光 (side backlight) / 轮廓光 (rim light) / 反射光，让主体有体积但不贴商业补光。

## 7. Negative 追加

在 v4 负面约束之后，按需追加：

```
no plastic skin, no CGI skin, no wax skin, no excessive beauty filter,
no sculpted AI body, no extreme hourglass silhouette, no malformed hands,
no warped anatomy, no duplicated limbs, no identity mixing, no studio posing,
no stiff front-facing lineup, no over-clean costume, no commercial beauty lighting,
no impossible rim light
```

## 8. V5 自检 (Self-check)

拒绝或重写当：

- 皮肤像蜡 / 塑料 / 磨皮，或全脸油亮
- 身体比例像雕塑 / AI，或关节错误、肢体重复
- 材质干净得像刚出厂，或痕迹是全局滤镜
- 湿 / 汗 / 尘与事件无关，或一镜堆满所有痕迹
- 空间像样板间 / 影棚，没有任何使用痕迹
- 不完美是统一贴纸，或出现 generative mistake
- 光线只有暖 / 冷两个形容词，没有时刻与来源
