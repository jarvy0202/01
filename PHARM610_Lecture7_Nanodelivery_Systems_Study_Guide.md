# PHARM 610 – Lecture VII：Nano-drug Delivery Systems 复习报告

> 授课：Dr. Afsaneh Lavasanifar（Midterm 2 范围的最后一讲）
> 资料：两段课堂录音 transcript（为主）+ Lecture VII PPT（为辅）
> 用法：从头读一遍就能知道老师讲了什么。每节最后的 **📝 Exam point** 是我判断最可能出 short answer 的点；文末有一整套「可能考题 + 英文答题模板」。
> 说明：transcript 是自动识别的，有很多拼写错误（"sublodextrin"=cyclodextrin，"Kylex"=Caelyx，"Onibet"=Onivyde，"aprexane"=Abraxane 等），下面都已更正。

---

## 0. 这节课讲什么（Learning Objectives）

老师开头说了这一讲的 4 个目标（PPT slide 2）：

1. 认识不同的 nano-delivery systems，重点是 **lipid-based**（liposome）和 **polymer-based**（polymeric nanoparticle、polymeric micelle）。
2. 描述这些系统 **最常用的制备方法（preparation methods）**。
3. 简单过一下表征方法（characterization）——老师说这部分已经在 Dr. Rakkei 的课上讲过了，这里只顺带提。
4. 认识每一类里 **临床上已有的制剂（clinically available formulations）** 以及它们的作用。

整节课的结构：

```
Nano-delivery systems
├── 1. 总体分类（biologic / polymeric / silicon / carbon / metallic）
├── 2. Cyclodextrins（最早的一类，solubilizer）
├── 3. Liposomes  ← 重点，占了约 2/3 的时间
│     ├── 结构 & 组成（phospholipid + cholesterol）
│     ├── 制备方法（film hydration / ethanol injection / microfluidics）
│     ├── 囊泡类型（SUV / LUV / MLV / MVV）& 设计类型（conventional / stealth / ...）
│     ├── 载药（passive vs active/remote loading → Doxil）
│     ├── Generic 审批要求（CQAs）、AF4、in vitro release
│     ├── Rapid vs Sustained release → PK 的改变
│     ├── Conventional vs Stealth（AmBisome, Myocet vs Doxil/Caelyx）
│     ├── Doxil 的 PK、毒性变化、hand-foot syndrome
│     ├── Onivyde（liposomal irinotecan）
│     ├── Active targeting（ligand、post-insertion、binding site barrier）
│     └── Triggered release（ThermoDox）
└── 4. Polymer-based systems
      ├── Polymeric nano/microparticles（材料、nanocapsule vs nanosphere、5 种制备方法、纯化、Abraxane）
      ├── Steric stabilization
      └── Polymeric micelles（形成机理、热力学、与 surfactant micelle 比较、载药方法、临床产品）
```

---

## 1. 纳米给药系统的总体分类（简要）

老师用一张表快速带过，**知道大类就行**：

| 类别 | 材料举例 | 纳米结构形式 |
|---|---|---|
| **Biologic（生物来源）** | lipids, peptides, nucleic acids, polysaccharides, viruses | vesicles（如 liposome）、nanoparticles |
| **Polymeric（合成高分子）** | PLA, PGA, PCL, poly(alkylcyanoacrylate), PEO, PEI | nanospheres, nanoparticles, micelles, dendrimers |
| **Silicon-based** | silicone, silicon dioxide | porous nanoparticles |
| **Carbon-based** | carbon | nanotubes, fullerenes（还有 nanodiamond） |
| **Metallic** | gold, silver, palladium, platinum | nanoparticles, nanoshells |

老师特别提了一句：**antibody–drug conjugates 和 polymer–drug conjugates 也被归类为 nanoscale drug delivery systems**。

（PPT 里那张各种系统尺寸对比图属于 FYI：nanoparticles 50–500 nm，microparticles 0.5–5 µm，liposomes 50–300 nm，dendrimers 1–20 nm，polymeric micelles 50–170 nm。）

---

## 2. Cyclodextrins（环糊精）

### 2.1 是什么
- 最早出现的纳米给药系统之一。
- **由葡萄糖（glucopyranose）单元连成的环状寡糖**（α-1,4 连接）。
- 按糖单元数分三种：

| 类型 | 糖单元数 |
|---|---|
| **α-cyclodextrin** | 6 |
| **β-cyclodextrin** | 7 |
| **γ-cyclodextrin** | 8 |

### 2.2 怎么工作
- 结构像一个"截顶的桶/甜甜圈"：**中间是疏水空腔（cavity），外面是亲水的**。
- 药物（疏水部分）钻进空腔，形成 **inclusion complex（包合物）**，从而增加药物水溶性。
- 可以形成 **1:1** 或 **1:2（drug : CD）** 等比例的复合物。
- 在环糊精表面可以接上不同的基团（例如 2-hydroxypropyl-β-CD、sulfobutylether-β-CD、randomly methylated β-CD），改变它对不同药物的亲和力。

```
        hydrophilic outside
         ___________
        /           \
       |   [drug]    |   <- hydrophobic cavity
        \___________/
   Drug + CD  <=>  Drug-CD inclusion complex (1:1 or 1:2)
```

### 2.3 老师的结论（重点）
- Cyclodextrins 作为 **solubilizing agent（增溶剂）非常成功**，很多产品上市了（PPT 上的产品清单是 FYI，不用背）。
- 但用于 **drug targeting 不成功**，原因是 **药物从 CD 中释放太快（fast release）**——包合是一个快速平衡，进到血液一稀释药物就跑出来了。

> 📝 **Exam point**：Cyclodextrin 的结构（α/β/γ = 6/7/8 个糖）、作用机制（疏水空腔形成 inclusion complex → 增溶）、为什么不能用于靶向（fast drug release）。

---

## 3. Liposomes（脂质体）——本讲重点

### 3.1 结构

- Liposome = 由 **phospholipid** 组成的 **囊泡（vesicle）**。
- 磷脂是两亲分子（amphiphilic）：一个亲水头（head group）+ 两条疏水脂肪酸尾巴（通过 glycerol 骨架连接）。
- 磷脂在水中自组装（self-assemble）成 **bilayer（双层膜）**，双层膜再闭合成 **vesicle** → 这就是 liposome。（磷脂也可以组装成 micelle，但形成囊泡的是双层结构。）

```
             PEG chains (stealth)          antibody/ligand (targeted)
               \  |  /                        Y
        .-~~~~~~~~~~~~~~~~~~~~~-.
       /  ooooooooooooooooooo    \     o = hydrophilic head
      |  o  ||||||||||||||||| o   |    | = hydrophobic tails
      |  o  |  AQUEOUS CORE  | o  |    <- lipid BILAYER: hydrophobic drugs
      |  o  |  (hydrophilic  | o  |
      |  o  |    drugs)      | o  |    <- aqueous core: hydrophilic drugs
      |  o  ||||||||||||||||| o   |
       \  ooooooooooooooooooo    /     interface: amphiphilic drugs
        '-~~~~~~~~~~~~~~~~~~~~~-'
```

**能装什么药：**
| 药物性质 | 装在哪里 |
|---|---|
| **Hydrophilic（水溶性）** | 中间的 **aqueous core** |
| **Hydrophobic（疏水）** | **lipid bilayer** 里 |
| **Amphiphilic（两亲）** | bilayer 和水相的 **界面** |

→ 这是 liposome 的一大优点：**三类药物都能装**。

### 3.2 组成成分

**Phospholipids（常见）：**
- Phosphatidylcholine（**PC**, lecithin，卵磷脂）
- Phosphatidylethanolamine（**PE**, cephalin，脑磷脂）
- Phosphatidylserine（PS）
- Phosphatidylinositol（PI）
- Phosphatidylglycerol（PG）
- 常常用几种磷脂的混合物。

**Cholesterol：**
- 几乎总会加。
- 作用：**增加双层膜的刚性（rigidity）→ 减少包载药物的泄漏（leakage）**。
- 也可以加其他亲脂衍生物插入 bilayer。

**磷脂结构如何影响性质：**
- **脂肪酸链不同 → 相变温度（transition temperature, Tm）不同**（链越长越饱和，Tm 越高，膜越"硬"）。
- **头基不同 → 功能不同**：
  - **Cationic lipids**（如 DOTAP、DOTMA）：带正电，帮助 liposome 与 **细胞膜 / 内体膜（endosomal membrane）** 融合、扩散。
  - **pH-dependent / ionizable lipids**（如 DLin-MC3-DMA）：pH 依赖性，**促进 endosomal escape**，并用于装载 **nucleic acids（如 RNA）**。
  - **PEG-lipids**（如 DSPE-PEG2000、DMG-PEG2000）：用于 stealth。

### 3.3 制备方法（Preparation methods）

**① Thin-film hydration method（薄膜水化法，传统方法）**

```
Lipid (+ lipophilic drug) dissolved in organic solvent
(chloroform / dichloromethane / chloroform + alcohol)
        │
        ▼  rotary evaporator 蒸掉溶剂
Thin lipid film on wall of round-bottom flask
        │
        ▼  加入水相（water / PBS，可含 hydrophilic drug）+ 搅动 (hydration/agitation)
Spontaneous formation of liposomes  → 多为 large MLVs（大、多层、不均一）
        │
        ▼  sonication（超声）/ extrusion（挤出）/ homogenization
Smaller, more homogeneous vesicles (SUVs)
```

- 缺点：得到的颗粒大、不均一，需要额外的 sonication/extrusion。老师说 **现在这个方法已经不太常用了**。

**② Ethanol injection method（乙醇注入法）**
- 脂质溶在 **ethanol** 中 → 把这个溶液 **注入水相**。
- 优点：直接得到 **更小、更均一** 的 liposome，很多时候 **不需要 extrusion/sonication**。实验室常用。

**③ Microfluidics（微流控）**——最新
- 让有机溶剂和水 **混合得更好**；
- 可以 **自动化、放大生产（larger scale）**。

### 3.4 囊泡类型（按层数和大小）

取决于 **脂质种类 + 制备方法**：

| 缩写 | 全称 | 特点 |
|---|---|---|
| **SUV** | Small Unilamellar Vesicle | 小、单层 |
| **LUV** | Large Unilamellar Vesicle | 大、单层 |
| **MLV** | Multilamellar Vesicle | 洋葱样多层同心膜 |
| **MVV** | Multivesicular Vesicle | 大囊泡里套多个小囊泡 |

```
  SUV      LUV         MLV            MVV
   o       ( )      ((( o )))     (  o  o  )
                                  ( o  o   )
```
可以用 fluorescence 或 electron microscopy 观察。

### 3.5 Liposome 的设计类型（Designs）

1. **Conventional liposomes**：表面没有任何修饰。
2. **pH-sensitive liposomes**
3. **Cationic liposomes**
4. **Thermo-responsive liposomes**
5. **Immunoliposomes**：表面接了 **antibody**。
6. **Long-circulating / Stealth liposomes**：表面有 **PEG**（或其他亲水聚合物），能逃避 mononuclear phagocytic system（MPS）。

另外按"代"来讲：表面接 PEG = stealth；表面接 ligand = actively targeted（second generation）。

### 3.6 载药方法（Drug encapsulation）

**① Passive loading（在制备过程中装药）**
- 药物溶于有机溶剂 → 加到有机相里（film hydration 或 ethanol injection 都可以）。
- 水溶性药物 → 放在水化用的水相里。

**② Active / Remote loading（主动/远程载药）**
- **先把 liposome 做好**，再把 liposome 和药物一起 **孵育（incubate）**。
- 关键：liposome 内部预先装了一个"东西"，能把药物 **从外面拉进里面**：
  - 一种 **buffer → 形成跨膜 pH 梯度**，药物进去后被离子化、溶解而留在里面；
  - 一种 **盐 → 与药物形成复合物并在 liposome 内部沉淀（precipitate）**。
- **例子：Doxil** ——内部是 **ammonium sulfate**（transcript 识别成 "aluminium sulfate"，应为硫酸铵），doxorubicin 进入后与 sulfate 形成复合物并 **沉淀/结晶**，于是 **doxorubicin 很难再泄漏出来**。
- 老师强调：这就是 **Doxil 至今仍是 PK 改变最显著、最成功的纳米制剂** 的原因——**药物泄漏极低**。

```
  外部 doxorubicin ──穿膜──►  [ (NH4)2SO4 inside ]
                             Dox + SO4²- → Dox-sulfate precipitate
                             → trapped, very low leakage
```

### 3.7 Generic liposome 的审批：Critical Quality Attributes（CQAs）

背景：Doxil 已过专利期，generic 公司可以生产。要保证 generic 与原研一致、**batch-to-batch uniformity**，监管机构需要以下标准：

1. **Lipid analysis** —— 脂质含量/浓度
2. **Drug encapsulation** —— 包封率
3. **Particle characterization** —— **particle size、polydispersity（PDI）、particle charge（zeta potential）**
4. **Stability** —— 聚集倾向（aggregation）、**shelf life**
5. **Drug release** —— 药物释放程度

> 📝 **Exam point**：列出 generic liposome（如 generic Doxil）需要满足的 quality criteria。

### 3.8 AF4：Field-Flow Fractionation（场流分离）

- 用于纳米颗粒的 **生产和纯化/分离**。
- 原理：颗粒在通道中随液体流动，**依靠流动（flow）把不同 size 的颗粒分开**；有的型号还加 **电场**，可以按 **charge** 分离；有的按 **size + density** 分离。
- **优点**：通道里 **没有 stationary phase（固定相）**，分离仅靠流动和颗粒的流动速度 → 对颗粒温和、不发生与固定相的相互作用。
- PPT 名称：**AF4 = Asymmetrical Flow Field-Flow Fractionation**。

### 3.9 In vitro drug release 测定

方法（PPT）：sample & separate、**dialysis membrane**、continuous flow、**reverse dialysis**。

老师讲的要点：
- 最常用 **dialysis**；现在也有尝试自动化，例如用 **USP Apparatus 2（paddle，常规片剂/胶囊溶出用）** 里放入 dialysis 装置。
- 两种取样方式：
  - 把纳米制剂放进释放介质，**从介质中取样**；
  - 如果释放出来的药浓度太低测不到 → 为 **每个时间点各放一个 dialysis 样品**，到时间取出一个，测 **bag 里剩下多少药**。
- 释放介质中常加 **surfactant 或 serum albumin**，作为结合位点/增溶剂，尤其对难溶药物 → 保证 **sink condition**。

### 3.10 临床 liposome 的时间线（FYI 为主）

- 大部分从 **1990 年代中期** 开始上市，到 2020 年有一批，适应症主要是 **抗癌药** 和 **抗真菌药**。
- **2020 年 mRNA vaccines** 上市——本质上是 **lipid nanoparticles（LNP）**，所用脂质类似前面列的那些。
- 时间线里要认得的：Doxil/Caelyx (1995)、AmBisome (1997)、Myocet (2000)、Visudyne (2000)、Onivyde (2015)、Onpattro (2018, lipid-siRNA)。

---

### 3.11 ★ Rapid release vs Sustained release liposome（核心概念）

**Rapid release formulations**
- 最早的 liposome 是 conventional 的，主要把 **疏水药物放在 lipid bilayer** 里。
- 药物在膜里 → **释放很快**，不能 sustained release → **PK 跟游离药差不多**。
- PPT 例子：**Visudyne**（verteporfin，药物在疏水膜内部）。

**Sustained release formulations**
- 药物 **不在 bilayer，而是被包在内部水相（encapsulated in liposome interior）**。
- **只有在这种情况下，载体才能改变药物的 PK 和 biodistribution（BD）**——药物不再按自己的 PK 走，而是"被迫"跟着 liposome 走。
- 结果：**副作用减少 + 药物更多到达作用部位 → therapeutic index ↑**
- Liposome 通过 **EPR effect** 外渗进入血管通透性高的病变组织（tumor、inflammation）。

**Therapeutic index 为什么升高？**（老师自问自答）
- 产生毒性的剂量 ↑（toxic dose goes up）
- 产生疗效的剂量 ↓（effective dose goes down）
- → TI = toxic dose / effective dose ↑

**药物 PK 与释放速度的关系（PPT slide 31，必考）：**

| 释放速度 | 药物的 PK 像谁 |
|---|---|
| 释放 **很慢**（如 Caelyx/Doxil） | **PK of drug ≈ PK of carrier** |
| 释放 **很快** | **PK of drug ≈ PK of free drug** |
| Sustained release liposome | **介于两者之间**：提前释放的那部分走 free drug 的 PK，仍在载体里的那部分走 carrier 的 PK |

```
 release rate:  fast ◄──────────────────────────► slow
 drug PK:     = free drug     (in between)     = carrier
 targeting:      none                         possible
```

> 老师的原话结论：**"The slower the release, the more similar the PK and BD of your drug to that of the carrier. That is why slow drug release is a prerequisite for achieving drug targeting."**
> （**缓慢释放是实现药物靶向的前提**）

---

### 3.12 ★ Conventional（classical）liposomes：例子与问题

**例子 1：AmBisome（amphotericin B）**
- Amphotericin B = **抗真菌药**；做成 **SUV liposome**；**1997 年批准**。
- Amphotericin B 是 **amphiphilic 药物**，主要位于 **lipid 与内部水相之间的界面**。
- 临床优势：**降低 amphotericin B 的肾毒性（nephrotoxicity）**。
- 老师把它作为 sustained-release liposome 的例子讲，但同时它是 **conventional**（没有 stealth 性质）。

**例子 2：Myocet（conventional liposomal doxorubicin）**
- 药物位于 liposome 的 **内部水相**。

**两者共同点**：都是 conventional liposome → **没有 stealth 性质 → 会被 mononuclear phagocytic cells 吞噬**。

**Conventional liposome 的命运（PPT 图）：**
- 血浆蛋白（opsonins）粘到"裸露"的 liposome 表面 → 被肝脏的巨噬细胞（**Kupffer cells**）摄取、破坏 → **tumor uptake 很低**。

**Conventional liposome 的主要问题：**
1. **Short circulation time** → 无法定位到病变组织（failure to localize to diseased tissues）
2. **High uptake into liver and spleen** → 重复给药可能损害肝脾功能（toxicity / impairment with repeat administration）

### 3.13 ★ Stealth liposomes

**机制：**
```
PEG (hydrophilic polymer) on surface
        │ absorbs water → hydration layer ("water coating")
        ▼
Blood proteins (opsonins) cannot adsorb to the surface
        ▼
Not recognized as "foreign" by MPS / Kupffer cells (seen as "self")
        ▼
Avoid uptake in liver & spleen → LONG-CIRCULATING
        ▼
(+ sustained release) → accumulate in tumors / inflammation via EPR
```

> 关键句：**If a liposome is BOTH stealth AND sustained-release, it can direct its cargo to disease sites such as solid tumors or inflamed areas.**

### 3.14 ★ Doxil / Caelyx（PEGylated liposomal doxorubicin）

| 项目 | 内容 |
|---|---|
| 名字 | **Doxil**（美国）= **Caelyx**（加拿大/欧洲） |
| 药物 | **Doxorubicin**（如卵巢癌化疗） |
| 类型 | **PEGylated（stealth）SUV liposome** |
| 粒径 | **~100 nm** |
| 组成 | **Hydrogenated soy phosphatidylcholine (HSPC) + cholesterol** + PEG-lipid |
| 载药 | Remote loading，ammonium sulfate 梯度 → 药物在内部沉淀 |
| 半衰期 | **长循环，t½ > 50 h（人体）** |
| 主要临床优势 | **降低毒性，尤其是 cardiotoxicity（心脏毒性）** |
| 对比 | Myocet = conventional liposomal doxorubicin |

**PK 变化（老师说对所有 sustained-release stealth nanocarrier 都可以这样预期）：**

Placing doxorubicin in stealth liposomes:
- **↓ Clearance**
- **↓ Volume of distribution (Vd)**
- **↑ Circulation half-life**
- **↑ AUC**
- **↑ Distribution to tumors**

PPT 图：同为 50 mg/m² 单剂量，Caelyx 血药浓度一直维持在 ~10–25 µg/mL 到 24 h；Adriamycin（游离 doxorubicin）几小时内就降到 ~0.1 µg/mL。

**为什么 Vd 下降？（常考计算/解释）**
- **Vd = Amount of drug in body (D_B) ÷ Plasma concentration (C_P)**
- 游离 doxorubicin：**Vd = 254 L**（远大于体液体积 → 药物大量分布到组织，包括正常组织）
- Liposomal doxorubicin：**Vd = 4.1 L ≈ 血液体积（~5 L）**
- 原因：liposome **太大，无法从正常组织的 continuous capillaries 外渗**，又因为 stealth 不被组织中的巨噬细胞摄取 → **药物被限制在血液中**。

**老师补充**：到今天为止，**Doxil 仍然是能够如此大幅改变药物 PK 的最好的制剂**，其他制剂都达不到，原因就是 **内部的 complexation/precipitation 使药物泄漏极少**。

**毒性的变化：**

| 降低的副作用（因为 liposome 不穿过正常血管） | 增加的副作用 |
|---|---|
| ↓ Cardiac toxicity（心脏毒性） | ↑ **Mucositis（黏膜炎）** |
| ↓ Hematological toxicities（血液毒性） | ↑ **Hand-foot syndrome**（palmar-plantar erythrodysesthesia, **PPE**） |
| Little or no hair loss（脱发少） | |
| ↓ Peripheral neuropathy | |
| No extravasation (vesicant) injuries | |
| ↓ Nausea & vomiting | |

- PPT：Caelyx vs free doxorubicin 的毒性谱 ≈ **continuous infusion vs bolus injection**（类似 5-FU、doxorubicin 持续输注时的毒性谱）。

**Hand-foot syndrome：**
- 机制（老师说"人们认为"）：手和脚是 **压力点（pressure points）**，压力使 liposome 被 **从血管里挤出来** → 药物在手足皮肤积累。
- PPT：剂量 **> 10–12 mg/m² per week** 时出现；影响受创伤的皮肤区域。
- 处理：出现毒性的第一迹象时，**推迟下一个化疗周期（delay the next cycle）**。

### 3.15 Onivyde（liposomal irinotecan）

- 约 10 年前上市（**2015**）。
- **Irinotecan（CPT-11）是 SN-38 的 prodrug**：
  - SN-38 的活性是 irinotecan 的 **~1000 倍**；
  - 但 **SN-38 水溶性差**，不能直接注射 → 所以做成水溶性 prodrug irinotecan。
  - **SN-38G（SN-38 glucuronide）** = 无活性代谢物。
- 做成 liposome 后，irinotecan 及其代谢物的 PK 都显著改变，**变化方向与 Doxil 类似**（AUC ↑、t½ ↑ 等）。PPT 图：120 mg/m² nal-IRI 的血药浓度比 300 mg/m² 普通 irinotecan 高得多、维持更久（到 ~160 h）。

---

### 3.16 Actively targeted liposomes（第二代：表面接 ligand）

**Internalizing vs non-internalizing ligands**
- Internalizing：ligand 结合的受体会 **内吞**，把 liposome 带进细胞内；
- Non-internalizing：liposome 只"坐"在细胞旁边，在细胞附近释放药物。
- 研究结果：**大多数情况下 internalizing ligands 效果更好**。

**Ligand 的选择：**
- **Full antibody（IgG）、antibody fragments（Fab'、scFv）、nanobodies**
  （targets 例：VEGFR、HER2/neu、CD19、CD20、CD22、CD33、CD25、CEA、MUC1 … FYI）
- **Aptamers**
- **Peptides**（RGD、NGR、YGSIR …）
- **Small molecules**（**folic acid/folate**）；其他：transferrin、IL-2、GM-CSF、lectins、galactosamine

**★ Passive vs ligand-mediated targeting —— 老师的结论（重点）：**
1. 文献证据：**接 ligand 并不会增加 liposome 在实体瘤中的蓄积（tumor localization）**——进入肿瘤主要还是靠 EPR（passive）。
2. 如果 **ligand 密度过高**，会 **遮盖 PEG 的 stealth 性质** → 被肝/脾/MPS 提前清除 → **血浆清除 ↑，肿瘤蓄积反而 ↓**。
3. Ligand 能改变的是 **肿瘤内部的分布（intratumoral distribution）**，例如增加细胞内摄取。

**★ Binding site barrier（结合位点屏障）：**
- 在 **大肿瘤** 中，带 ligand 的 liposome 会被 **第一层（靠近血管的）肿瘤细胞抓住** → 不能渗透到肿瘤核心。
- 肿瘤越大，屏障越大。
- **微转移（micrometastatic disease）或血管内的靶点** 障碍更少 → 更适合 ligand-targeted liposome。

### 3.17 Post-insertion technique（后插入法）

```
Ligand (e.g., anti-CD19) coupled to PEG-phospholipid (MAL-PEG-DSPE)
        │  这些 PEG-lipid 自组装成 micelles
        ▼
Ligand-PEG-lipid micelles + pre-formed liposomes (e.g., Caelyx)
        │  co-incubate (PPT: 37 °C, 1 h)
        ▼
Ligand-PEG-lipids insert into the OUTER leaflet of the liposome
        → targeted stealth liposome (e.g., anti-CD19-targeted Caelyx)
```

- **为什么比"传统方法"好？** 传统方法是把 ligand-lipid 与其他磷脂一起混合，再做 film hydration 或 ethanol injection —— 这样一部分 ligand 会 **朝向 liposome 内部**，被藏起来、浪费掉。Post-insertion 只插入外层，**更多 ligand 暴露在表面**。

### 3.18 Triggered release liposomes：ThermoDox

- 在 liposome 中加入 **温度敏感的脂质（lysolipid）**。
- 设计：**37 °C 稳定 → 局部加热到 42 °C** 时发生相变，膜变得通透 → doxorubicin 在加热的肿瘤处快速释放。
- 2000 年代初引起很大关注。
- **结果失败**：后来发现它 **在 37 °C 时也不能有效防止泄漏** → 没能在商业化道路上走远。

> 📝 **Exam point（liposome 部分）**：
> - 三类药物在 liposome 中的位置；cholesterol 的作用
> - film hydration / ethanol injection / microfluidics 的步骤和优缺点
> - active (remote) loading 的原理，以 Doxil 为例
> - conventional liposome 的两个问题；stealth 的机制
> - 为什么 sustained release 是 targeting 的前提；release rate 与 PK 的关系
> - Doxil 的 5 项 PK 变化 + Vd 254 L → 4.1 L 的解释
> - Doxil 毒性 ↓ 与 ↑；hand-foot syndrome 的机制和处理
> - ligand targeting 不增加肿瘤蓄积；binding site barrier；post-insertion 的优点
> - ThermoDox 为什么失败

---

## 4. Polymer-based micro/nanoparticles（聚合物纳米/微粒）

### 4.1 材料

| Natural macromolecules | Synthetic polymers |
|---|---|
| Gelatin | **PLA**（poly(lactic acid)） |
| **Albumin** | **PGA**（poly(glycolic acid)） |
| Alginates | **PLGA**（poly(lactic-co-glycolic acid)） |
| | **PCL**（poly(caprolactone)） |
| | PACA（poly(alkyl cyanoacrylate)） |
| | PMMA |

### 4.2 两种设计：Nanocapsule vs Nanosphere

```
   Nanocapsule (reservoir)          Nanosphere (matrix)
     .-----------.                    .-----------.
    /  polymer    \                  /  .   .  .   \
   |   .-----.     |                |  .  polymer . |
   |   | DRUG|     |                |   .   .   .   |
   |   '-----'     |                 \  .  .   .   /
    \  shell      /                   '-----------'
     '-----------'               drug dispersed throughout
  drug core + polymer shell
```

- **Nanocapsule**：药物在中心形成核（core），外面一层聚合物壳 → reservoir system。
- **Nanosphere**：药物均匀分散在聚合物基质中 → matrix system。

### 4.3 五种制备方法（重点）

**① In situ polymerization（原位聚合）**
- 由 **单体（monomer）** 直接在体系中聚合形成颗粒。
- **Emulsion polymerization**：有机相（与水不混溶）和水相；initiator 在一相，monomer 在另一相（或反之）；可以是 continuous organic phase 或 continuous aqueous phase；用 **surfactant 防止聚集**。
- **Interfacial polymerization**：在两相界面上聚合。

**② Coacervation（凝聚法）**
- 主要用于 **microparticles**，能做 **reservoir（储库型）系统**。
- 步骤：聚合物溶于有机溶剂，药物颗粒分散其中形成核 → 加入 **non-solvent（通常是水）** → 聚合物析出形成 **coacervate**，包裹在药物颗粒周围 → **蒸发溶剂**，coacervate 硬化成包衣。

```
(a) drug particles  →  (b) + polymer solution  →  (c) add non-solvent:
    polymer coacervate deposits on drug  →  (d) solvent removed: hardened coating
```

**③ Emulsification / solvent evaporation（乳化-溶剂蒸发法）** —— **PLGA 粒子最常用**
- **水相**：含 surfactant 或 **PVA（polyvinyl alcohol）** 作为稳定剂。
- **有机相**：聚合物溶于 **与水不混溶的溶剂（water-immiscible）**，如 **chloroform**、DCM。
- 两相不混溶 → 形成 **emulsion**：
  - **O/W emulsion** → 用于 **水不溶性（hydrophobic）药物**；
  - **W/O/W（double emulsion）** → 用于 **水溶性（hydrophilic）药物**。
- 蒸发有机溶剂 → 形成纳米粒，表面包有 surfactant/PVA 起稳定作用。

**④ Solvent displacement（溶剂置换法，nanoprecipitation）**
- 与 ③ 的区别：有机相是 **与水混溶（water-miscible）** 的溶剂：**acetone**，或其他极性溶剂（THF、acetonitrile 等）。
- 聚合物溶于有机相 → 与水混合 → **水作为 non-solvent** 使聚合物析出成颗粒 → 蒸发有机溶剂。
- 也常用于 PLGA；**得到的颗粒比 emulsion 法更小**。

**⑤ Precipitation by salting out（盐析法）**
- 与 ④ 相似，区别：在水相中加入 **electrolyte（电解质）**，靠 **salting out** 触发颗粒形成；随后加大量蒸馏水稀释。

**对比小表：**

| 方法 | 有机溶剂 | 关键点 | 适用 |
|---|---|---|---|
| In situ polymerization | 视情况 | 从 monomer 聚合 | — |
| Coacervation | 有机溶剂 + 加 non-solvent | polymer coacervate 包裹 drug core | microparticles，reservoir |
| Emulsion/solvent evaporation | **water-immiscible**（chloroform） | O/W（疏水药）或 W/O/W（亲水药），PVA 稳定 | PLGA |
| Solvent displacement | **water-miscible**（acetone, THF, ACN） | 水为 non-solvent，颗粒更小 | PLGA |
| Salting out | water-miscible | 水相加 electrolyte 触发 | — |

### 4.4 纯化（Purification）——去除未包封的游离药物

| 方法 | 原理 | 备注 |
|---|---|---|
| **Dialysis** | 透析膜让小分子游离药通过 | 水溶性药用水相介质；溶于有机溶剂的药可用有机溶剂（前提是不破坏颗粒）或混合溶剂。**缺点：透析过程中药物可能迁移到颗粒表面 → 之后出现 burst release（突释）** |
| **Ultrafiltration** | 半透膜（水平放置）+ **真空或离心** 加速 | 例：**Amicon filters** |
| **Ultracentrifugation** | 颗粒沉淀到底部，游离药留在 **supernatant** | |
| **GPC / Size exclusion chromatography** | **Sephadex** 柱：**大颗粒先流出**，小分子进入凝胶孔隙后流出 | |

### 4.5 Abraxane（nab-paclitaxel）

- **Human serum albumin–bound paclitaxel** 纳米粒（albumin nanoparticle，~130 nm）。
- **2005 年批准**（breast cancer）。
- 老师重点：**与 Doxil 不同，它并没有按 stealth 制剂预期的那样改变药物 PK**，但它在多种癌症中 **确实有效**，上市时是一个 **breakthrough**。

### 4.6 Steric stabilization（空间稳定）

- 定义：**在递送系统表面引入亲水性高分子（hydrophilic macromolecules）**，防止颗粒聚集（aggregation）。基于热力学（ΔG = ΔH − TΔS），老师说细节不讲。
- 两种方式：
  - **Physical adsorption（PEO coating）**：用 PVA，或含 PEG 的嵌段共聚物吸附在颗粒表面，如
    - **Pluronics**：**PEO-PPO-PEO triblock** copolymer
    - **PEO-PLA diblock** copolymer
  - **Chemical attachment（PEO grafting）**：把 PEG 化学接到颗粒表面。

---

## 5. Polymeric micelles（聚合物胶束）

### 5.1 形成与结构

- **Amphiphilic block copolymer**（一段亲水、一段疏水）在浓度 **高于 CMC（critical micelle concentration）** 时自组装成 **core–shell** 结构 → polymeric micelle。
- **尺寸约 100 nm**（slide 图标注 ~100 nm）。
- **Shell**：亲水段，通常是 **PEG（PEO）**，很致密。
- **Core**：疏水段 → 装 **poorly water-soluble drugs**。
- 用途：**增溶难溶药物**，也可用于 **难溶药物的靶向递送**。

```
          ~~~ ~~~ ~~~           ~~~ = hydrophilic block (PEG) -> SHELL
       ~~~  \  |  /  ~~~
     ~~~ ---( CORE  )--- ~~~     core = hydrophobic blocks + drug
       ~~~  /  |  \  ~~~
          ~~~ ~~~ ~~~
                ~100 nm
```

常用的 block copolymers：
- PEO-*b*-PPO（Pluronic）
- **PEO-*b*-PLA**
- PEO-*b*-poly(L-amino acid)（如 poly(aspartic acid) 衍生物）
- （还有 PEO-*b*-PCL）

### 5.2 ★ 胶束化的热力学：Hydrophobic effect（必考）

**公式：ΔG = ΔH − TΔS**；自发过程需要 **ΔG < 0**。

**在水中（aqueous）：**
- 胶束化通常是 **endothermic（吸热，ΔH > 0）**；
- 因此必须靠 **ΔS 增大（entropy-driven）** 才能让 ΔG < 0。

**熵从哪来？——水的结构：**
1. 水分子之间通过 **hydrogen bonds** 形成三维网络结构。
2. 亲水段可以和水形成氢键；**疏水段不能**，它 **破坏了水的三维氢键网络**（疏水段周围的水被迫更有序 → 熵低）。
3. 为了重新获得熵，水倾向于把疏水段 **"赶出去"（expel）**。
4. 当疏水段聚到一起形成 core（藏起来不接触水），水分子之间的三维氢键网络得以重建，**水的熵增加** → ΔS > 0 → ΔG < 0 → 过程自发、热力学有利。

**在有机溶剂中：** 胶束化是 **enthalpy-driven（exothermic）**。

```
 unimers in water: water ordered around hydrophobic blocks (low S_water)
         │  hydrophobic blocks associate into core
         ▼
 micelle: those water molecules released → free H-bond network (high S_water)
 ΔH > 0 (small), TΔS > ΔH  →  ΔG < 0  → spontaneous
```

### 5.3 ★ Polymeric micelles vs Low-MW surfactant micelles

| 比较 | Polymeric micelles | Surfactant micelles（如 Cremophor EL, SDS, polysorbates） |
|---|---|---|
| **CMC** | **很低** —— 疏水段是大分子，聚集/被水排斥的倾向更强 | 较高 |
| **Core** | **刚性（rigid）**，大分子链之间相互作用 | 类液体（liquid-like） |
| **Kinetic stability** | **高**：低于 CMC 时解离也很慢（**> hours**），药物释放慢（min–hrs） | 低：**毫秒级** 快速解离 |
| 静脉注射稀释后 | CMC 很低 → 稀释后可能仍高于 CMC；即使低于 CMC 也解离很慢 | 迅速解离，药物马上释放 |
| 结果 | 有可能实现 **IV 给药后的 sustained release 和 targeting** | 只能增溶 |

> 两个原因（老师原话结构）：**(1) lower CMC (thermodynamic stability)；(2) better kinetic stability (rigid core)**。

### 5.4 载药方法（Encapsulation methods）

1. **Dialysis method**：聚合物和药物溶于 **DMSO 或 DMF** → 对水透析 → 水逐步置换有机溶剂 → 形成胶束并载药。
2. **O/W emulsion method**：**先做好胶束**（例如用 solvent displacement）→ 把药物溶在 **与水不混溶的溶剂（chloroform）** 中加入 → **剧烈搅拌** → 药物进入 core → 蒸发 chloroform。
3. **Solvent evaporation / film hydration**（与 liposome 类似）：药物 + 聚合物溶于 selective solvent（如 methanol）→ 蒸干成膜 → 加水 → 载药胶束。
4. **Co-solvent evaporation（= solvent precipitation/displacement）**：用 **与水混溶、低沸点** 的溶剂（**acetone**；也可 acetonitrile、THF）溶解聚合物和药物 → 加入水中（或把水 **逐滴** 加入有机相）→ 蒸发 acetone → 得到载药胶束。
5. **Microfluidics**：现在也用于胶束自组装（如 PCL-*b*-PEO + paclitaxel，DMF 体系）。

### 5.5 进入临床的 polymeric micelles

| 产品 | 组成 / 药物 | 结局 & 要点 |
|---|---|---|
| **NK911** | PEG–poly(aspartic acid)（部分 doxorubicin 共价连接）+ **物理包载 doxorubicin**；日本研发 | 做到临床试验，但 **PK 远不如 liposomal doxorubicin（Doxil）**（AUC、t½ 都低很多，虽比 free DOX 好）→ **竞争不过 Doxil，被淘汰** |
| **SP1049C** | **Pluronic**（F127 : L61 = 8:1）的 **doxorubicin** 胶束 | 目标是 **drug-resistant cancers**；获 orphan drug status（食管、上消化道、胃癌）；**最终没达到目的，被淘汰** |
| **NK105** | **Paclitaxel** 包在 PEG–modified polyaspartate 胶束中 | **最有希望**：PK 变化符合预期——AUC 大幅 ↑、t½ ↑、Cmax ↑、Tmax ↑（肿瘤）、CL ↓、Vss ↓；动物中疗效好、神经毒性低；**但人体中没达到预期终点（PD 没有预期的改善）** |
| **Genexol-PM** | **PEG–PDLLA**（mPEG-poly(D,L-lactide)）**paclitaxel** 胶束 | **成功上市**：使 paclitaxel 溶解度比 **水中溶解度高 ~5000 倍**；**没有 Taxol 中 Cremophor EL 带来的毒性**；在 **韩国和印度** 临床使用；曾进入美国做临床，但 **Abraxane 的生产公司收购了该公司，消除了 Abraxane 在美国的竞争** |
| 同一聚合物的 **docetaxel** 胶束 | PEG–PDLLA + docetaxel | 也在 **韩国和印度** 上市 |

NK105 关键数据（PPT，FYI 看趋势即可）：plasma AUC 309 → 15,566 µg·h/mL（~50×），CL 323.6 → 6.4 mL/h/kg，Vss 812 → 55 mL/kg；tumor AUC 331 → 7,965（~24×），Tmax 0.5 → 6 h。
NK911 vs L-DOX：AUC 3,263 vs 902,000 ng·h/mL；t½β 2.8 h vs 45.9 h；CL 6.7 vs 0.02 mL/min/kg。

> 📝 **Exam point（polymer 部分）**：nanocapsule vs nanosphere；5 种制备法（尤其 O/W vs W/O/W 选择、immiscible vs miscible 溶剂区别）；纯化方法及 dialysis 的缺点；steric stabilization 定义；micelle 的结构、CMC；**hydrophobic effect / entropy-driven 的解释**；polymeric vs surfactant micelles 的两点差异；载药方法；Genexol-PM 的优势；NK911/NK105 为何失败。

---

## 6. 全讲最核心的 10 个"一句话"

1. **Cyclodextrins**：疏水空腔包合药物 → 好的 solubilizer，但 **fast release → 不能 targeting**。
2. **Liposome** 可装亲水（core）、疏水（bilayer）、两亲（interface）药；**cholesterol ↑ rigidity ↓ leakage**。
3. **Remote loading（Doxil）**：先成囊，内部 ammonium sulfate 使 doxorubicin **沉淀** → 极低泄漏 → Doxil 至今 PK 改变最大。
4. **只有 sustained release（药在 aqueous core）才能改变药物 PK/BD**；**slow release is a prerequisite for drug targeting**。
5. **Conventional liposomes**：被 MPS（Kupffer cells）清除 → 循环短、肝脾蓄积。
6. **Stealth（PEG）**：水化层阻止 opsonin 吸附 → 长循环 → EPR 进肿瘤/炎症部位。
7. **Doxil**：CL↓、Vd↓（254 L → 4.1 L ≈ 血容量）、t½↑（>50 h）、AUC↑、tumor 分布↑；心脏毒性↓，但 **mucositis 和 hand-foot syndrome ↑**。
8. **Ligand targeting 不增加肿瘤蓄积**，高密度 ligand 会破坏 stealth；只改变 intratumoral distribution；大肿瘤有 **binding site barrier**；用 **post-insertion** 接 ligand。
9. **Polymer NP 制备**：O/W（疏水药）vs W/O/W（亲水药），immiscible（emulsion）vs miscible（solvent displacement，粒子更小）。
10. **Polymeric micelles**：hydrophobic effect（**entropy-driven，endothermic**）；比 surfactant micelles **CMC 更低 + kinetic stability 更高**；唯一真正上市的是 **Genexol-PM（PEG-PDLLA paclitaxel）**。

---

## 7. 可能考题 & 英文答题模板（Short-answer practice）

> 答案写得比考试要求略完整，考试时挑关键词写即可。

**Q1. What are cyclodextrins and how do they increase drug solubility? Why have they not been successful for drug targeting?**
Cyclic oligosaccharides of 6 (α), 7 (β) or 8 (γ) glucopyranose units with a hydrophilic exterior and a hydrophobic central cavity. Poorly soluble drugs (or their hydrophobic parts) enter the cavity to form 1:1 or 1:2 drug–CD inclusion complexes, increasing aqueous solubility. They failed for targeting because drug release from the complex is very fast (rapid dissociation upon dilution in vivo), so the drug does not follow the carrier.

**Q2. Where are hydrophilic, hydrophobic and amphiphilic drugs located in a liposome? Why is cholesterol added?**
Hydrophilic → aqueous core; hydrophobic → lipid bilayer; amphiphilic → bilayer/water interface (e.g., amphotericin B in AmBisome). Cholesterol increases bilayer rigidity and reduces leakage of the encapsulated drug.

**Q3. Describe the thin-film hydration method. How can the size of the liposomes be reduced?**
Lipids (± lipophilic drug) are dissolved in an organic solvent (chloroform/DCM) → solvent removed by rotary evaporation to form a thin lipid film → film hydrated with aqueous buffer (± hydrophilic drug) with agitation → liposomes (mostly large MLVs) form spontaneously. Size reduced and homogenized by sonication or extrusion (or homogenization).

**Q4. Compare thin-film hydration with ethanol injection and microfluidics.**
Ethanol injection: lipid in ethanol injected into aqueous phase → smaller, more homogeneous liposomes, often without extrusion/sonication. Microfluidics: better controlled mixing of organic and aqueous phases, automated and scalable. Film hydration gives large heterogeneous MLVs requiring downsizing and is now used less.

**Q5. What is active (remote) loading? Give an example.**
Liposomes are formed first, then incubated with the drug; an entity pre-loaded inside (a buffer creating a pH gradient, or a salt) drives the drug from outside to inside and traps it (ionization or complexation/precipitation). Example: Doxil – an ammonium sulfate gradient; doxorubicin forms a sulfate complex that precipitates inside the liposome, greatly reducing leakage.

**Q6. List the critical quality attributes a generic liposomal product (e.g., generic Doxil) must meet.**
Lipid analysis (lipid concentration), drug encapsulation efficiency, particle characteristics (size, polydispersity, charge), stability (aggregation, shelf life), and drug release – to ensure batch-to-batch uniformity and similarity to the brand product.

**Q7. What is field-flow fractionation (AF4) and what is its advantage?**
A technique to separate nanoparticles by size (and density, or charge if an electric field is applied) based only on their movement in a laminar flow and a cross-flow in a channel. Advantage: no stationary phase, so separation depends only on flow – gentle, no interaction with packing material.

**Q8. How is in vitro drug release from nanocarriers measured? Why is surfactant or albumin added to the medium?**
Dialysis (bag/device, can be placed in USP apparatus 2), sample-and-separate, continuous flow, reverse dialysis. Either sample the release medium, or, if released drug is too dilute, use one dialysis sample per time point and measure the drug remaining inside. Surfactant or serum albumin acts as a solubilizer/binding sink for poorly soluble drugs to maintain sink conditions.

**Q9. Compare rapid-release and sustained-release liposomal formulations. Why is slow drug release a prerequisite for drug targeting?**
Rapid release: hydrophobic drug in the bilayer, released quickly → PK ≈ free drug (e.g., Visudyne). Sustained release: drug encapsulated in the aqueous interior → only in this case are PK/BD changed by the carrier. If release is very slow, PK of drug ≈ PK of carrier; very fast, PK ≈ free drug; sustained-release systems lie between. The slower the release, the more the drug follows the carrier to the target site, so slow release is required for targeting.

**Q10. Explain how a sustained-release liposome can increase the therapeutic index.**
The drug follows the liposome, which accumulates at disease sites (tumor, inflammation) by the EPR effect and avoids normal tissues. Higher drug levels at the site of action lower the effective dose; less exposure of normal tissues raises the toxic dose → TI (toxic dose/effective dose) increases.

**Q11. What are the main problems with conventional (classical) liposomes? Give examples.**
Plasma proteins (opsonins) adsorb to the naked surface → uptake by the mononuclear phagocytic system (Kupffer cells in liver, spleen) → short circulation time and failure to localize in diseased tissue; high liver/spleen uptake → possible impairment/toxicity with repeated administration. Examples: Myocet (doxorubicin), AmBisome (amphotericin B).

**Q12. How do stealth liposomes avoid MPS uptake?**
Surface-grafted hydrophilic polymer (PEG) binds water to form a hydration layer that prevents adsorption of blood proteins/opsonins; the liposome is not recognized as foreign by macrophages → reduced liver/spleen uptake → long circulation → accumulation in tumors/inflamed tissue via EPR (if also sustained release).

**Q13. Describe Doxil/Caelyx. What PK changes occur when doxorubicin is placed in stealth liposomes?**
PEGylated (stealth) SUV liposomes of doxorubicin, ~100 nm, HSPC + cholesterol, remote-loaded; t½ > 50 h in humans; main clinical benefit is reduced cardiotoxicity. PK: ↓ clearance, ↓ Vd, ↑ half-life, ↑ AUC, ↑ distribution to tumors.

**Q14. Why does the volume of distribution of doxorubicin decrease from 254 L to 4.1 L in Doxil?**
Vd = amount in body / plasma concentration. Free doxorubicin distributes extensively into tissues (high Vd). Liposomes are too large to extravasate through continuous capillaries of normal tissues and, being stealth, are not taken up by tissue macrophages, so the drug is confined to plasma; Vd ≈ blood volume (~5 L).

**Q15. Which side effects of doxorubicin decrease and which increase with Doxil? What is hand-foot syndrome and how is it managed?**
Decreased: cardiotoxicity, hematological toxicity, hair loss, peripheral neuropathy, vesicant injuries, nausea/vomiting. Increased: mucositis and hand-foot syndrome (palmar-plantar erythrodysesthesia). HFS is thought to arise because hands and feet are pressure points where liposomes are squeezed out of capillaries; seen at > 10–12 mg/m²/week; managed by delaying the next chemotherapy cycle at the first sign of toxicity.

**Q16. Why is Doxil the most successful formulation in changing drug PK?**
Because the drug is complexed/precipitated (doxorubicin-sulfate) inside the stealth liposome, leakage is extremely low, so the drug follows the carrier's long-circulating PK.

**Q17. What is Onivyde? Why is irinotecan used instead of SN-38?**
PEGylated liposomal irinotecan (2015). Irinotecan is a water-soluble prodrug of SN-38; SN-38 is ~1000× more potent but too poorly water soluble to inject. Liposomal formulation changes the PK of irinotecan and its metabolites (SN-38, inactive SN-38G) similarly to Doxil (↑ AUC, ↑ t½).

**Q18. Does attaching a targeting ligand increase tumor accumulation of liposomes? Explain.**
No – evidence shows tumor localization is governed by EPR (passive). High ligand density may mask the stealth PEG layer → faster MPS clearance → lower tumor accumulation. Ligands may change intratumoral distribution (e.g., cell internalization); internalizing ligands generally work better than non-internalizing ones.

**Q19. What is the binding site barrier?**
In large tumors, ligand-targeted liposomes bind to the first layer of tumor cells near the vessels and are trapped there, preventing penetration into the tumor core. The larger the tumor, the greater the barrier; micrometastases or intravascular targets present fewer barriers.

**Q20. Describe the post-insertion technique and why it is preferred.**
Ligands are coupled to PEG-phospholipids (e.g., MAL-PEG-DSPE), which form micelles; these are co-incubated with pre-formed (conventional or PEGylated) liposomes (e.g., 37 °C, 1 h) and the ligand-lipids insert into the outer leaflet. Preferred over mixing ligand-lipid with other lipids before film hydration/ethanol injection because more ligand is exposed on the outer surface instead of facing the interior.

**Q21. What is ThermoDox and why did it fail?**
A thermosensitive (lysolipid-containing) liposomal doxorubicin designed to undergo a phase transition and release drug rapidly when heated from 37 to 42 °C (local hyperthermia). It failed because it was not effective at preventing doxorubicin leakage at 37 °C.

**Q22. Distinguish nanocapsules and nanospheres.**
Nanocapsule = reservoir: drug core surrounded by a polymer shell. Nanosphere = matrix: drug dispersed throughout the polymer matrix.

**Q23. Describe the emulsification/solvent evaporation method. When would you use O/W vs W/O/W?**
Polymer (e.g., PLGA) dissolved in a water-immiscible organic solvent (chloroform) is emulsified into an aqueous phase containing PVA or surfactant; the solvent is evaporated, leaving nanoparticles stabilized by PVA/surfactant. O/W for water-insoluble drugs; W/O/W (double emulsion) for water-soluble drugs.

**Q24. How does solvent displacement differ from emulsion/solvent evaporation and from salting out?**
Solvent displacement uses a water-miscible organic solvent (acetone, THF, acetonitrile); water acts as non-solvent and precipitates the polymer; gives smaller particles than emulsion methods. Salting out is similar but particle formation is triggered by electrolytes in the aqueous phase.

**Q25. Describe coacervation.**
Mainly for microparticles/reservoir systems: polymer is dissolved in an organic solvent containing dispersed drug particles; a non-solvent (water) is added so the polymer separates as a coacervate that deposits around the drug core; the solvent is evaporated and the coating hardens.

**Q26. List methods to purify nanoparticles from unencapsulated drug. What is a drawback of dialysis?**
Dialysis, ultrafiltration (Amicon, vacuum or centrifugation), ultracentrifugation (particles pellet, free drug in supernatant), size exclusion chromatography/GPC (Sephadex; large particles elute first). Dialysis drawback: drug can migrate to the particle surface during dialysis, causing burst release later.

**Q27. What is Abraxane and how does it differ from Doxil?**
Human serum albumin-bound paclitaxel nanoparticles (nab-paclitaxel), approved 2005 (breast cancer). Unlike Doxil it does not change the PK of the drug as expected for stealth carriers, yet it is clinically effective and was a breakthrough.

**Q28. What is steric stabilization and how is it achieved?**
Incorporation of hydrophilic macromolecules on the surface of a delivery system to prevent particle aggregation. Achieved by physical adsorption of PVA or PEG-containing block copolymers (Pluronic PEO-PPO-PEO, PEO-PLA) or by chemical grafting of PEG.

**Q29. Describe the structure of polymeric micelles and their use.**
Amphiphilic block copolymers above the CMC self-assemble into core–shell structures (~100 nm): dense hydrophilic PEG shell, hydrophobic core. Used to solubilize poorly water-soluble drugs and potentially for targeted delivery.

**Q30. Explain the thermodynamics (hydrophobic effect) of micellization in water.**
ΔG = ΔH − TΔS; spontaneous if ΔG < 0. In water micellization is usually endothermic (ΔH > 0), so it must be entropy-driven. Hydrophobic blocks cannot hydrogen-bond with water and disrupt its 3D hydrogen-bond network, ordering surrounding water (low entropy). Expelling hydrophobic blocks into a micelle core restores the water network and releases ordered water, increasing entropy so TΔS > ΔH and ΔG < 0. In organic solvents micellization is enthalpy-driven (exothermic).

**Q31. Why are polymeric micelles more stable in blood than low-MW surfactant micelles?**
(1) Much lower CMC (macromolecular hydrophobic block → stronger tendency to associate), so after dilution in blood they may remain above CMC. (2) Greater kinetic stability: the rigid core of interacting polymer chains dissociates slowly (hours) even below CMC, vs milliseconds for liquid-like surfactant cores (Cremophor EL, SDS, polysorbates). This allows sustained release and potential targeting after IV injection.

**Q32. Describe two methods for loading drugs into polymeric micelles.**
Dialysis: polymer + drug dissolved in DMSO/DMF, dialyzed against water so water replaces the solvent and micelles form with drug. Co-solvent evaporation: polymer + drug in a water-miscible low-boiling solvent (acetone/ACN/THF), mixed with water (or water added dropwise), solvent evaporated. (Also: O/W emulsion – preformed micelles + drug in chloroform with vigorous mixing then evaporation; film hydration; microfluidics.)

**Q33. Name polymeric micellar formulations that reached the clinic and their outcomes.**
NK911 (PEG–poly(aspartic acid)/doxorubicin, Japan) – PK inferior to Doxil, abandoned. SP1049C (Pluronic F127/L61 doxorubicin, for drug-resistant cancer) – failed. NK105 (paclitaxel, PEG–modified polyaspartate) – expected PK changes (↑AUC, ↑t½, ↓CL) and good animal data but did not meet clinical endpoints. Genexol-PM (PEG–PDLLA paclitaxel) – marketed in South Korea and India.

**Q34. What are the advantages of Genexol-PM over Taxol?**
PEG–PDLLA micelles increase paclitaxel solubility ~5000-fold over its water solubility without Cremophor EL, avoiding the Cremophor-related toxicity of Taxol.

---

## 8. 跳过 / 只需略知的 FYI 内容

以下内容老师只是展示或一带而过，我判断不会出 short answer，所以没有展开：
- Cyclodextrin 的发现历史年表、上市产品清单（Sporanox、Vfend 等）
- Liposome 商业时间线上每个产品的年份（只需记住 Doxil 1995、AmBisome 1997、Onivyde 2015、mRNA LNP 2020）
- 各种磷脂/阳离子脂质的化学结构式
- 抗体靶点的完整清单（VEGFR、HER2、CD20…）
- NK911 / NK105 PK 表中的具体数值、SP1049C 的 orphan drug 适应症
- 微流控芯片的具体构造
