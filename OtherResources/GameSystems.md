# 🎮 Game Systems Taxonomy

Uma taxonomia prática de **sistemas de jogo**, organizada por **género** e **caso de uso**, com foco em padrões arquiteturais recorrentes.

---

# 🧠 1. Sistemas Fundamentais (Cross-Genre)

## Lógica e Fluxo
- **Finite State Machine (FSM)**
  - Player states (idle, run, jump, attack)
  - AI states (patrol, chase, attack)
- **Hierarchical State Machine (HFSM)**
  - Estados compostos (ex: Combat → Melee / Ranged)
- **Behavior Trees (BT)**
  - Alternativa à FSM para AI complexa
- **GOAP (Goal-Oriented Action Planning)**
  - AI baseada em objetivos dinâmicos

## Controlo
- **Input Abstraction Layer**
  - Mapping (keyboard/controller → actions)
- **Character Controller System**
  - Física vs kinematic movement
- **Camera Control System**
  - Follow, orbit, lock-on

## Core Loop Systems
- **Game Loop (Update / FixedUpdate / Render)**
- **Event System / Message Bus**
- **Entity Component System (ECS)** ou **OOP-based Actors**

---

# 🧙 2. RPG / Action RPG

## Progressão
- **Experience & Leveling System**
- **Skill Tree / Talent System**
- **Stat System (STR, DEX, INT...)**
- **Scaling System (enemy/player balance)**

## Combate
- **Ability System (cooldowns, mana, effects)**
- **Damage Calculation System**
- **Status Effects System (buffs/debuffs)**

## Inventário
- **Inventory Grid / Slot System**
- **Equipment System**
- **Loot Generation (procedural / tables)**

## Mundo
- **Quest System (FSM-driven ou data-driven)**
- **Dialogue System (branching trees)**

---

# 🔫 3. FPS / Shooter

## Combate
- **Weapon System**
  - Hitscan vs Projectile
- **Recoil System**
- **Bullet Physics / Ballistics**

## Percepção
- **Aim Assist / Targeting System**
- **Hit Detection System**
- **Damage Feedback System (hit markers, sound)**

## Movimento
- **Player Movement FSM**
  - Walk / Sprint / Crouch / Slide
- **Cover System (opcional)**

---

# 🧠 4. Strategy (RTS / Turn-Based)

## Tempo
- **Turn System (turn queue, initiative)**
- **Real-Time Tick System**

## Gestão
- **Resource Management System**
- **Production / Build Queue System**

## Unidades
- **Unit Command System (orders, pathfinding)**
- **Group AI / Formation System**

## Mundo
- **Fog of War System**
- **Grid / Tile System**

---

# 🏎️ 5. Racing / Simulation

## Física
- **Vehicle Physics System**
- **Traction / Drift Model**
- **Collision System**

## Controlo
- **Input Smoothing System**
- **Assist Systems (ABS, traction control)**

## Corrida
- **Lap System**
- **Checkpoint System**
- **AI Driving System (racing lines)**

---

# 🧩 6. Puzzle / Casual

## Lógica
- **Rule Engine**
- **Grid State System**

## Progressão
- **Level Unlock System**
- **Scoring System**

## Conteúdo
- **Procedural Level Generator (opcional)**

---

# 🕵️ 7. Stealth / Immersive Sim

## AI
- **Perception System (vision cones, sound)**
- **Suspicion State Machine**
  - Idle → Suspicious → Alert → Combat

## Mundo
- **Systemic Interaction System**
  - Ex: fogo propaga, luz influencia stealth

## Player
- **Visibility System**
- **Noise System**

---

# 🧱 8. Sandbox / Survival

## Simulação
- **Hunger / Thirst System**
- **Day/Night Cycle**
- **Weather System**

## Construção
- **Crafting System**
- **Building System (grid ou freeform)**

## Recursos
- **Resource Gathering System**
- **Inventory + Weight System**

---

# 🧠 9. AI Systems (Detalhado)

## Arquiteturas
- **FSM (simples, previsível)**
- **Behavior Trees (modular)**
- **Utility AI (score-based decisions)**
- **GOAP (planeamento dinâmico)**

## Sensores
- **Line of Sight**
- **Hearing System**
- **Memory System (last seen position)**

---

# ⚙️ 10. Sistemas Técnicos de Suporte

## Infraestrutura
- **Save/Load System**
- **Scene/Level Streaming**
- **Networking System (client-server, rollback)**

## Telemetria
- **Analytics System**
- **Debug Tools / Dev Console**

---

# 🧭 Como usar isto na prática

## Ordem recomendada
1. **Core Loop**
2. **Player FSM**
3. **Input + Camera**

## Depois
- 1 sistema principal do género (ex: combat, puzzle rules)

## Só depois
- Progressão / meta systems
