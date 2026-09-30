# SRC Brief 2 — OCR / Transcription of `SRC_BRIEF.md` Images

This document is a text reconstruction (OCR + visual description) of every image embedded in
[SRC_BRIEF.md](/home/wang/projects/kage/SRC_BRIEF.md). The images come from two sources:

1. Frame grabs from a presentation/video about a "Film DNA" cinematic-website design system
   (dark "film-set HUD" style slides, mixed English/Chinese).
2. Screen recordings of an editor scrolling through a source file called
   `FILM_DNA_PROJECT_BRIEF.md`, plus a couple of reference tool/website screenshots
   (Claude Code skill install log, Canvas UI, React Bits).

Website referenced at the top of the original brief: https://www.alayendo.com/

---

## Part 1 — "Film DNA System" Presentation Slides

### Slide: `image.png` — Film DNA System / 叙事化网站工作流 (Narrative Website Workflow)

HUD-style title bar reads `FILM DNA SYSTEM` / `叙事化网站工作流` with fake camera telemetry
(timecode, FPS 24.00, shutter 172.8°, iris f/2.8, ISO 800, WB 3200K).

- **灵感来源（输入）/ Inspiration sources (input):**
  1. **Kage** — *camera choreography* / 镜头运动与调度灵感 (camera movement & blocking inspiration)
  2. **WebGL 网站** — *depth and transitions* / 深度、空间与转场灵感 (depth, space & transition inspiration)
  3. **Canvas UI** — *glass / liquid / shatter* / 材质表现与交互灵感 (material & interaction inspiration)
- **工作流主轴（转化为叙事化网站）/ Main workflow axis (converting into a narrative website):**
  `Story` (故事/情绪/意图) → `Shot` (镜头语言/镜头调度) → `Visual Technique` (视觉技巧/风格/质感)
  → `Implementation` (网站实现/交互落地)
- **思考的转折点 / 从模仿到叙事 (Turning point in thinking / from imitation to narrative):**
  > 我不是直接复制这些效果。("I'm not directly copying these effects.")
  > 我会先问：这个 technique 在我的故事里代表什么？("I first ask: what does this technique represent in my story?")
- **核心结论 / 叙事驱动的交互原则 (Core conclusion / narrative-driven interaction principle):**
  > 每一次滚动动画的时候，都应该像一次 camera decision。
  > ("Every scroll/animation should feel like a camera decision.")
- Film-strip thumbnails labeled `FLOATING FRAMES / 灵感碎片` (floating frames / inspiration fragments).
- Footer HUD: `LOOK: FILM 2383`, `FORMAT: 2.39:1`, `COLOR: KODAK 2383`, `PROJECT: NARRATIVE WEB`, `ROLL: A001`, `SCENE: 03`, `TAKE: 07`.

### Slide: `image-1.png` — Film DNA · Camera Thinking

- Headline: **它不是十几个场景，而是一部长镜头。** ("It's not a dozen scenes, it's one long take.")
- Subtext: 用户滚动，实际上是在控制一台摄影机，穿过一个持续存在的 3D 世界。
  ("When the user scrolls, they are actually controlling a camera moving through a persistent 3D world.")
- Camera HUD readout: `CAMERA 01`, `24 FPS`, `180°`, `F/2.8`, `00:00:12:08`, scroll position ruler `-2 … 0 … +2`.
- Boxed rule (the site's most important rule):
  > 这是我整个 Film DNA 网站最重要的一条规则：
  > **EVERY SCROLL SHOULD FEEL LIKE A CAMERA DECISION.**
- Footer tags: 持续世界 · 摄影机路径 · 电影感体验 · 用户驱动叙事
  (Persistent world · Camera path · Cinematic experience · User-driven narrative)
- **Scroll → camera-move mapping table (right column), each paired with a still + purpose:**
  | Input | Camera move (EN/中文) | Purpose (中文) |
  |---|---|---|
  | SCROLL 滚动 | — | — |
  | ↓ | DOLLY IN 推进 | 镜头向前推进，进入故事空间 / 建立沉浸感，拉近观众与世界的距离 |
  | ↓ | ORBIT 环绕 | 镜头环绕观察，展现世界的维度 / 建立空间关系，提供更多信息 |
  | ↓ | PASS THROUGH 穿越 | 镜头穿过元素，进入下一个层次 / 转场与过渡，推动故事向前 |
  | ↓ | PULL BACK 拉远 | 镜头拉远，建立整体格局 / 总结情绪，留下思考与余韵 |
- Bottom filmstrip timeline from `START` to `END` with caption 从头到尾 ("from start to finish") and
  footer line: 不是页面切换，而是镜头运动。不是跳转，而是电影。
  ("Not page switches, but camera movement. Not jumps, but film.")

### Slide: `image-2.png` — 把 Three.js 原则抽成 Skills (Turning Three.js Principles into Skills)

- Headline: **把 Three.js 原则抽成 Skills** — 不是解释几百行 shader，而是把反复使用的判断，沉淀成 `reusable context`。
  ("Turn Three.js principles into Skills — not explaining hundreds of lines of shader, but distilling
  repeatedly-used judgment calls into reusable context.")
- Central hub node: **Reusable Context — AI SKILLS SYSTEM**
- Four primary skill cards around the hub:
  - **A — cinematic-scroll-world** (负责/handles): persistent scene, normalized scroll, camera keyframes, section handoff
  - **B — camera-director** (负责): dolly, orbit, push-through, FOV, composition
  - **C — webgl-atmosphere** (负责): fog, particles, restrained bloom, grain, vignette
  - **D — film-dna-design** ("The Light Shapes Memory.") (负责): dark cinematic palette, serif + mono, film language, blob rules, visual hierarchy
- Three secondary skill nodes below: **material-transition** (morph/dissolve/merge/split),
  **visual-router** (choose web/image/video), **visual-review** (QA/compare/refine)
- Quote at bottom: "AI coding 真正变强的地方，不是 prompt 写得越来越长，而是……reusable context。"
  (captioned live subtitle: "然后就是 Web WebGL 的氛围系统" — "then there's the Web/WebGL atmosphere system")
- Footer breadcrumb: `Three.js Skills / Film DNA / AI Workflow`

### Slide: `image-3.png` — Claude Code skill-install session log (screenshot of chat/tool output)

Plain light-mode screenshot of an agent's tool-run summary while setting up this very project:

```
Ran 4 commands
Installing project-local into .claude/skills/:
Ran 2 commands, created CLAUDE.md +51 -0
Installed — 10 skills, project-local.

.claude/skills/
├── cinematic-scene-director        (00)
├── cinematic-world-builder         (01)
├── scroll-camera-director          (02)
├── procedural-environment-builder  (03)
├── webgl-dom-depth-composer        (04)
├── cinematic-atmosphere-lighting   (05)
├── cinematic-post-processing       (06)
├── environmental-particles         (optional)
├── foreground-transitions          (optional)
└── threejs-performance-review      (QA)
```

Details text below the tree:
- "Flat, not nested. I stripped the zip's `00-`…`09-` prefixes so each folder name matches the
  skill's `name:` frontmatter — that's what discovery keys on. Verified all 10 match. The 00-06 /
  optional / QA hierarchy is encoded as invocation order in the new `CLAUDE.md`, where I also mapped
  each phase to the folder it owns in `src/` (01 → src/world/, 02 → src/camera/, 05/06 → src/atmosphere/,
  04 → src/dom/)."
- "Docs copied to `docs/cinematic-web-director-usage.md` and `docs/PROJECT_BRIEF.template.md`."
- "Project-local, per the kit's own recommendation. If you want these in every project instead,
  they'd go in `~/.claude/skills/` — say the word and I'll copy them there too."
- Note: "the source zip is in your iCloud Trash, so it may be purged — the installed copies are now
  the only ones, and this isn't a git repo, so they're unversioned. Second, skills added mid-session
  aren't picked up until Claude Code reloads..."
- "Next step would be phase 00: fill in `docs/PROJECT_BRIEF.template.md` for Film DNA, then run
  `cinematic-scene-...`" (cut off)
- Overlaid caption: "我自己的 film DNA 的 design" ("my own Film DNA design")

### Slide: `image-4.png` — Film DNA · Product Philosophy

- Headline: 我的产品核心是从 **Prompt Interface → Production Interface**。
  ("The core of my product is going from a Prompt Interface to a Production Interface.")
- Five-step visual metaphor of a glass pane with a prompt suspended inside it, cracking apart:
  1. **PROMPT SUSPENDED IN OPTICAL GLASS** — glass pane holding text "Create a cinematic mysterious motel thriller at night…"
  2. **CAMERA PUSH-IN**
  3. **CRACK** — glass begins to fracture
  4. **SHATTER** — glass shatters into shards
  5. **PRODUCTION VARIABLES FLY OUT** — shards become labeled tags: Character DNA, Environment DNA,
     Camera DNA, Color DNA, Continuity Lock, Motion DNA, Composition DNA, Time & Pace, etc.
- Quote: "所以我没有用一个普通 headline 来解释这个。我让产品思想本身成为 `transition`。"
  ("So I didn't use an ordinary headline to explain this. I made the product idea itself become the transition.")
- **技术 BREAKDOWN (technical breakdown)** icons: DOM Typography (内容语义清晰/可访问性强) +
  WebGL Glass Plane (光学玻璃质感/真实折射) + Fracture Geometry (动态裂纹算法/可交互可控) +
  Scroll Timeline (滚动驱动时间线/用户控制节奏) + Camera Push (镜头推进/沉浸式体验)
- Comparison panel: **如果用 AI VIDEO (if using AI video)** — 只能播放一次，用户无法控制
  (plays only once, user has no control) **VS 用 WEBGL (using WebGL)** — 用户控制裂纹发生的速度，
  每一次滚动都是不同体验 (user controls the crack speed, every scroll is a different experience)
- Bottom bar: 滚动控制裂纹的发生 (scroll controls when cracks occur), speed scale `SLOW ⟷ FAST`
  labeled 用户滚动速度 = 裂纹发展速度 (user scroll speed = crack growth speed)
- Live caption overlay: "就是我有这个 prompt interface" ("so I have this prompt interface")
- HUD footer: `CAMERA FOV 38mm`, `SHUTTER 180°`, `FPS 24.00`, `TIME CODE 00:00:12:08`, `DOLLY IN`

### Slide: `image-16.png` — Film DNA · Decision Framework

- Headline: 什么时候该用 WebGL，什么时候该用生成模型？ ("When should you use WebGL vs. a generative model?")
- Flowchart:
  - `Visual idea` → `Can the browser render it?`
    - **YES** → `Three.js / WebGL / CSS / SVG` (浏览器原生实现 — native browser implementation)
    - **NO** → `Does it need a realistic still?`
      - **YES** → `Image model` (静态真实画面 — realistic still image)
      - **NO** → `Does it need realistic motion?`
        - **YES** → `Video model` (真实动态镜头 — realistic motion shot)
- Live caption: "有一些呃这种2D的动画" ("there are some, uh, this kind of 2D animation")
- Side labels: `CREATIVE DECISIONS / CLEAR PATHS`, `EVALUATE / CHOOSE / CREATE`, `FOCUS ON STORY`,
  `VER. 1.0`, footer tagline: 想法先行 · 路径清晰 · 工具正确 — "RIGHT TOOL. RIGHT STORY."
  Corner tag: "MADE FOR FILMMAKERS / BY FILMMAKERS"

### Slide: `image-17.png` — Film DNA / 构建原则 · 5 条规则 (5 Build Principles)

Headline: **5 条规则** (5 Rules), subtitled THREE.JS 网站构建 / 电影 DNA / 构建原则.

1. 先参考，再编码。 — Reference first, then code.
2. 每一次滚动，都是一次镜头决策。 — Every scroll is a camera decision.
3. 让每个 WebGL 效果都承担叙事角色。 — Every WebGL effect must carry a narrative role.
4. 只生成那些浏览器无法做得更好的部分。 — Only generate the parts the browser can't do better natively.
5. 把好的决策，沉淀为可复用的技能。 — Distill good decisions into reusable skills.

Footer: 构建美感。讲述故事。交付体验。("Build beauty. Tell a story. Deliver an experience.")
Channel credit: `YOUTUBE.COM/@PIXELCINEMA`; scene slate reads `场景 05 / 镜次 规则 / 开拍 THREE.JS`.

---

## Part 2 — Reference Tool / Library Screenshots

### `image-5.png` — Canvas UI docs site (canvas-ui component library)

Left sidebar nav: `Canvas UI`, sections `Components` (Browse All, ASCII Object, ASCII Sweep, Asciify,
**Bend** [selected], Blaze, Bubble, Canvas, Cloth, Clouds, Decrypt Reveal, Dithered Object,
Displacement, Droplets, Flame Wrap, Force Field…), bottom button `Playground`.
Main panel shows the **Bend** component demo: "Scroll to watch the photo bend over the fold along
with the rest of the page," a wildflower-meadow photo rendered with a warped/bent edge, an
**Install** section with npm/pnpm/yarn/bun tabs and command `npx shadcn@latest add @canvas-ui/bend-react`.
Top-right icons: mail, search, theme toggle, GitHub star count `4.2k`.

### `image-6.png` — React Bits (Pro components) site

Top nav: `React Bits / DOCS / TOOLS / PRO / SPONSORS`, GitHub star count `45.9k`. Left sidebar:
Get Started (Introduction, Installation, MCP, Index), Pro (Components, Blocks, App UI, Templates,
Agent Kit), Tools (Background Studio, Shape Magic, Texture Lab), Text Animations (Masked Heading,
Particle Text, Split Flap Text…). Grid of component preview cards, several tagged `NEW`: **Aurora
Beam**, **Aurora Blur**, **Bending Marquee**, **Black Hole**, **Blinking Dots** (with `View live`
button), **Blinking Squares**, **Blur Highlight**, **Blurred Rays**, **Card Spread**. Right sidebar:
sponsor callouts for Shadcnblocks.com (Diamond) and shadcncraft (Silver). Live caption overlay:
"就是你可以预览啊这种" ("so you can preview this kind of thing").

---

## Part 3 — Reconstructed Source Document: `FILM_DNA_PROJECT_BRIEF.md`

The remaining images (`image-7`, `image-19`, `image-8`, `image-9`, `image-10`, `image-20`,
`image-11`, `image-18`, `image-12`, `image-13`, `image-14`, `image-15`) are sequential screenshots of
an editor auto-scrolling through a file named `FILM_DNA_PROJECT_BRIEF.md` (path shown in the tab:
`Users > meiyang > Desktop > Film DNA 1 codex > FILM_DNA_PROJECT_BRIEF.md`). Stitching them together
by their visible line numbers reconstructs almost the entire document, transcribed below. A few short
spans were not captured by any screenshot (scrolled past too quickly) and are marked `[...]`.

> Note: `image-20` and `image-15` are exact duplicate frames of `image-10` and `image-11`
> respectively (repeated/paused frames in the source recording).

```markdown
# Film DNA Landing Page — Project Brief

## Product
**Film DNA**

An AI-native cinematic production system that turns directorial intent into structured, reusable
production decisions across characters, environments, camera, lighting, motion, continuity, style,
and generation workflows.

Film DNA is not positioned as another prompt box or model marketplace. It is positioned as a
**directorial intelligence layer / creative control protocol** that helps creators make coherent
films instead of isolated generations.

## Audience

### Primary
- AI filmmakers
- commercial directors
- creative directors
- small film studios
- advertising agencies
- visual storytellers
- advanced creators producing cinematic AI video

### Secondary
- creators who want professional-looking film outputs but do not understand cinematography
  terminology, prompt engineering, camera systems, continuity, or model-specific controls
- teams that need repeatable visual consistency across many shots
- agencies that need a structured system for turning creative direction into production-ready
  generation

The landing page should speak to both experienced visual creators and less technical creators.

## One-sentence promise

**Turn creative intent into a coherent film production system — without relying on prompt
engineering.**

Alternative shorter brand line:

**Build the film, not the prompt.**

## Primary CTA

**Start Building Your Film DNA**

Secondary CTA:

**Explore the System**

Optional demo-oriented CTA:

**See How Film DNA Works**

The primary CTA should feel like entering a production environment, not opening a generic AI
generator.

## Narrative transformation

### From:
- repeatedly rewrite prompts
- switch between different generation models
- lose character consistency
- lose environmental continuity
- struggle to reproduce camera language
- manually remember lighting, lenses, motion, style, and visual rules
- regenerate shots without understanding why they failed
- depend heavily on model-specific prompt tricks

### To:
A structured, production-first workflow where Film DNA:
- captures directorial intent
- converts creative decisions into structured DNA
- preserves continuity across scenes and shots
- maps references intentionally
- recommends or routes to appropriate generation models
- makes cinematic variables understandable and reusable
- helps non-experts make better directorial decisions
- gives advanced users deeper control without requiring prompt-heavy workflows
- turns individual generations into part of one coherent production system

The emotional transformation should feel like:

**Chaos → Structure → Direction → Control → Production**

## Required chapters / content

### 1. Hero — The End of Prompt-First Filmmaking
Purpose: Establish Film DNA as a different category from prompt-based AI video tools.

Core idea: A prompt is visible as a fragile, flat interface or object. It feels limited and
temporary.

Suggested copy direction:
[... a few lines not captured by any screenshot ...]
- camera slowly approaches a prompt-like surface
- prompt surface begins to fracture / separate / reveal depth
- visitor moves through the prompt into the Film DNA world

Narrative role: **Old paradigm → threshold**

### 2. DNA System — Every Cinematic Decision Becomes Structured
Purpose: Introduce the central Film DNA concept.

Show major DNA categories such as:
- Character DNA
- Environment / World DNA
- Camera DNA
- Lighting DNA
- Color DNA
- Motion DNA
- Style DNA
- Spatial DNA
- Continuity DNA
- Edit DNA
- Sound / Voice DNA as future or extended capability

Core message:

Film DNA does not treat a film as one giant prompt.

It decomposes filmmaking into controllable, understandable production variables.

Interaction idea:
DNA nodes or cards exist spatially inside the world. As the camera travels through them, individual
systems become visible and connect into a larger production structure.

Narrative role: **Fragments → cinematic language**

### 3. Directorial Intelligence — You Do Not Need to Know Every Variable
Purpose: Prevent the product from feeling overly technical or only for professional directors.

Introduce:
- Semantic Inputs
- Ask Director
- guided recommendations
- intent-to-DNA translation
- presets / starting points
- reference-aware suggestions

Example:

A user can say:

> "I want this scene to feel lonely, elegant, restrained, and slightly unsettling."

Film DNA can translate that intent into relevant choices involving:
- lens
- framing
- camera distance
- lighting
- palette
- movement
- environment
- performance
- pacing

Core message:

**You direct with intent. Film DNA helps translate that intent into production decisions.**

### 4. Production Memory + Continuity — One Film, Not Hundreds of Separate Generations
[... section intro not captured by any screenshot ...]
- Continuity Locks
- Identity Lock
- Spatial Lock
- scene / shot inheritance
- versioning
- repair
- consistency evaluation

Visual idea:
Multiple shots appear around a persistent production graph. Character, environment, lens, light, and
spatial decisions remain connected across shots.

Core message:

Film DNA remembers what the production has already decided.

A new shot should inherit the film's rules instead of starting from zero.

Narrative role: **Individual generation → persistent production**

### 5. Scene Graph + Spatial DNA — Understand the World, Not Just the Image
Purpose: Reveal that Film DNA understands relationships between elements in a scene.

Introduce:
- Scene Graph
- Spatial DNA
- subject relationships
- blocking
- foreground / midground / background
- camera-to-subject relationships
- world continuity
- object placement
- shot-to-shot spatial reasoning

Visual idea:
Camera enters a spatial scene graph in which nodes are not abstract decoration but represent real
production relationships.

Core message:

Film DNA can preserve not just how something looks, but **where it is, how it relates to the
camera, and how the scene is constructed.**

Narrative role: **Image → world model**

### 6. Model Intelligence — The Model Is a Tool, Not the Product
Purpose: Separate Film DNA's value from any single image/video model.

Introduce:
- Model Intelligence Layer
- capability matching
- routing
- hard / soft requirements
- compatible / degraded / incompatible outcomes
- manual override with constraints
- future provider support through APIs such as fal or direct model integrations

Core message:

Film DNA decides what the shot requires first.

Then it can determine which model is most appropriate.

The model can change. The directorial system remains.

Visual idea:
A production specification travels through a routing structure toward different model endpoints
while the DNA remains unchanged.

Narrative role: **Model dependency → model independence**

### 7. Production Compiler — From DNA to Generation-Ready Instructions
Purpose: Explain how structured decisions become executable.

Conceptual pipeline:

**Creative Intent**
→ **Film DNA**
→ **Production Shot Spec**
→ **Requirements**
→ **Model Intelligence**
→ **Compiler**
→ **Generation**
→ **Evaluation / Repair**

[... a short span not captured by any screenshot ...]

Narrative role: **Direction → execution**

### 8. Output / Reveal — A Production System for AI Filmmaking
Purpose: Pull everything together.

Camera pulls back and reveals that the individual DNA systems, scene graph, continuity memory,
model intelligence, and production compiler are all parts of one connected operating system.

Suggested final statement:

**The future of AI filmmaking is not better prompting.
It is better direction.**

or:

**One creative language.
One production memory.
Any generation model.**

Primary CTA:

**Start Building Your Film DNA**

Narrative role: **System reveal → action**

## Visual DNA

### mood
[... one or two mood words not captured by any screenshot ...]
- restrained
- mysterious
- editorial
- premium
- tactile
- filmic
- technological without looking like generic SaaS
- futuristic without becoming cyberpunk
- immersive but controlled

The experience should feel closer to:

**film title sequence + cinematography + editorial design + realtime interactive installation**

than:

**AI SaaS dashboard landing page**

### palette

Primary:
- near black
- charcoal
- deep graphite
- slightly warm black

Secondary:
- bone white
- muted silver
- soft grey

Accent:
- restrained warm amber
- dark red / vermilion
- subtle tungsten warmth

Optional environmental contrast:
- desaturated cold blue / blue-grey for depth
- warm practical light for focal elements

Avoid bright saturated rainbow gradients.
```

*(The document continues beyond this point in the source recording, but no further images capture
additional content.)*

---

## References (from original brief)

- https://mengto.github.io/kage/
- https://www.usavionix.com/
- https://www.deepwhite-gallery.com/
- https://austinwerner.io/
