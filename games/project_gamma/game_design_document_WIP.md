# Starbound Voyager - Game Design Document (WIP)

**Status**: Living Document - Evolving Through Collaborative Design Process  
**Last Updated**: 2025-08-01  
**Design Phase**: Core Vision Complete, Detailed Mechanics In Progress  

---

## 🎯 PROJECT OVERVIEW

**Working Title**: Starbound Voyager  
**Genre**: Top-down Space Roguelite / Exploration Survival  
**Platform**: PC (Steam)  
**Development**: Solo Developer  
**Target Audience**: Fans of roguelites, exploration games, and strategic resource management  

---

## ✅ CORE VISION (ESTABLISHED - BUT STILL EVOLVING)

### Best Player Moment
**Vision**: Seeing run success leading to meaningful upgrades that add options/variety (not just power increases), plus upgrades to the universe/world itself.

**Key Design Principles**:
- Upgrades fundamentally change HOW you explore and gather resources
- Not just power increases - new options, ways to overcome challenges, varied experiences
- Upgrades to the universe/world unlock new content and experiences

### Core Appeal - "Runaway Train" Feeling
**Vision**: Player feels out of control but finds control within each stop. Mystery destination adds narrative potential.

**Design Elements**:
- Being on a runaway train going somewhere potentially amazing
- Finding measure of control within constraints
- Perfect for indie game storytelling and narrative
- Tension between helplessness and agency

### Design Balance - Evolving POI System
**Vision**: Early game frustration becomes late game empowerment through POI evolution (like Path of Exile map shaping).

**Mechanics**:
- Players can add more POIs between runs
- Influence what appears in different system types
- Specialization creates control over galaxy generation
- Transforms early limitations into progression goals

---

## ✅ CORE GAMEPLAY LOOP (ESTABLISHED)

1. **Arrival** - Ship jumps to new system with time limit
2. **Scanning** - Player discovers POIs (initially manual, upgrades to automated)
3. **Exploration** - Active piloting to gather resources and explore
4. **Combat** - Defensive encounters with rogue AI drones (if present)
5. **Management** - Resource allocation, upgrades, ship maintenance
6. **Jump** - Automatic progression to next system when time expires

---

## ✅ UPGRADE SYSTEM PHILOSOPHY (ESTABLISHED)

### Exploration Upgrades Progression
- **Manual scanning** → **System-wide scans** → **Future system prediction** (1,2,3 systems ahead)
- Shows: star class, POI counts, time ranges, system modifiers
- Specialization upgrades increase certain POI types in specific star colors

### Resource/Gathering Upgrades
- New materials accessible through upgrades
- Exotic materials lock higher tier upgrades (upgrades lead to upgrades)
- New gathering, refining, utilization capabilities

### System Influence Mechanics
- Players CAN'T control ship's path in a run
- CAN influence probability of star colors, POI types, system effects through upgrades
- Example: Specialize in Blue star + moon mining = more of those spawn

### Progression Philosophy
- **Story progress separate** - required upgrades as story gates/tier unlocks
- **Upgrade paths create tension** - specializing locks out other paths or increases costs
- **Permanent per character upgrades**
- Examples: Moon breaking, deep core mining, probe scanning, scanning arrays

---

## ✅ STORY & PROGRESSION STRUCTURE (ESTABLISHED)

### Story Gate Structure
- **Distance-based** progression with key encounters at specific jump numbers
- Key encounters reveal secrets about:
  - Ancient space-traveling alien race (derelict stations, ships, tech throughout galaxy)
  - Rogue AI drones (enemy threat, origins, purposes, mechanics)

### Specialization System
- **Soft locks** (increased costs, not hard blocks)
- Players can pursue multiple paths but must consider cost/benefit
- Option to overprep and grind more to access multiple paths

### Exotic Materials
- **RNG drops** from specific sources:
  - Specific asteroid types
  - Moon types
  - Anomaly types
  - Derelict alien ship/station salvage
- **Upgrades increase success chance up to 50%** (open to discussion)
- **Bad luck protection** ensures players don't go too long without rewards

---

## ✅ COMBAT SYSTEM FRAMEWORK (ESTABLISHED)

### Combat Trigger & Flow
- **Some systems defended by rogue AI drones**
- **Upgrades reveal drone presence** in future systems (part of prediction system)
- **Drones don't attack immediately** - sometimes delayed
- **30-second warning** shuts down all ship operations for defense prep
- **Ship destruction = run over**

### Damage System Architecture
**Three-Layer Defense**:
1. **Shields** → **Armor** → **Hull**
2. Ship destroyed when hull HP reaches 0
3. **While shields hold**: Ship systems take NO damage
4. **While taking armor damage**: Ship systems have chance of damage
5. **While taking hull damage**: Much higher chance of system damage

### System Damage Consequences
Critical ship systems and their failure states:
- **Life Support offline** → Death timer starts
- **Drone Bay offline** → Can't launch mining drones
- **Sensors offline** → Can't run scans
- **Communication Array offline** → Can't send scanner probes
- **Primary Engines offline** → Can't jump (death if jump timer reaches 0)
- **Refinery offline** → Can't refine materials
- **Matter Processor offline** → Can't produce food + death timer

### Combat Mechanics Philosophy
**Defensive Focus** (inspired by Wall World/Dome Keeper):
- **Defensive upgrades**: Shield strength, shield recharge speed, armor, etc.
- **Active abilities**: Different types of weapons and defensive tools
- **Energy system**: Powers combat abilities, part of upgrade progression

**Combat Specialization Potential**:
- **Fortress Build**: Heavy shields/armor, energy-efficient defense
- **Evasion Build**: Fast recharge, mobility-based abilities
- **Berserker Build**: Minimal defense, devastating offense

---

## 🔄 DETAILED MECHANICS (ACTIVELY BEING DESIGNED)

### Energy System Details
**Status**: Framework established, specifics needed
- Energy powers combat abilities
- Part of upgrade progression
- **Open Questions**:
  - How does energy regeneration work during combat?
  - Should energy capacity vs regeneration be separate upgrades?
  - How do different specializations affect energy systems?

### Enemy Design & Variety
**Status**: Concepts established, details needed
- **Visually different enemy types** with distinct behaviors
- **Damage immunities** and resistances
- **Attack patterns** players learn over time
- **Priority targeting** decisions
- **Enemy interactions**: Some buff others, time-sensitive threats
- **Open Questions**:
  - How many enemy types for launch version?
  - Progression of enemy complexity through the journey?
  - Non-lethal ways to learn enemy weaknesses?

### Ability Types & Trees
**Status**: Categories identified, trees need design
- **Mouse-targeted weapons**: Fire at cursor location
- **Auto-targeting weapons**: Used on cooldowns
- **AOE abilities**: Energy pulses to damage/disable/disrupt
- **Energy management**: Strategic resource for combat abilities
- **Open Questions**:
  - Should abilities be locked to specialization paths?
  - Shared abilities vs. specialization-exclusive abilities?
  - How do abilities scale with upgrades?

### Cross-System Synergies
**Status**: Concepts identified, implementation needed
- Damaged sensors could reduce weapon accuracy
- Life support upgrades extend death timers
- Drone bay upgrades could provide combat support
- **Integration Points**: How upgrades affect multiple systems

---

## ❓ AREAS NEEDING EXPLORATION

### Resource Economy Balance
**Priority**: High
- Material types and conversion rates
- Storage limits and inventory management
- Scarcity curves and progression pacing
- Trade-offs between different resource types

### POI Content Design
**Priority**: Medium
- Specific encounter types for different POIs
- Reward structures and risk/reward balance
- Environmental storytelling opportunities
- Procedural variation within POI types

### Temporal Mechanics Balance
**Priority**: Medium
- Jump timer lengths and variation
- Combat duration balancing
- Preparation time vs exploration time
- How different builds affect timing

### Audio/Visual Direction
**Priority**: Medium-Low
- Art style specifics and visual identity
- UI/UX design principles
- Audio design and atmosphere
- Visual feedback for game systems

---

## 📝 PLACEHOLDER SECTIONS (NOT YET TACKLED)

### Technical Architecture
- Engine choice and implementation details
- Performance considerations
- Save system and progression persistence
- Procedural generation algorithms

### User Interface Design
- HUD layout and information hierarchy
- Menu systems and navigation
- Accessibility considerations
- Controller vs keyboard/mouse support

### Audio Design
- Music and atmosphere
- Sound effects and feedback
- Audio accessibility features
- Dynamic audio systems

### Marketing & Distribution
- Target audience refinement
- Platform strategy
- Marketing messaging
- Community building approach

### Localization & Accessibility
- Text localization planning
- Visual accessibility features
- Audio accessibility considerations
- Cultural sensitivity review

---

## 🎯 DESIGN TENSIONS & CHALLENGES

### Identified Tensions (Need Ongoing Balance)
- **Resource Allocation**: Repairs vs. immediate upgrades when systems are damaged
- **Risk/Reward**: Offensive upgrades (faster clearing) vs. defensive upgrades (safer exploration)
- **Specialization**: System redundancy vs. focused builds
- **Time Pressure**: Risk one more run vs. prepare for combat
- **Complexity**: Rich systems vs. accessible gameplay

### Key Balance Points
- Energy system complexity vs. intuitive gameplay
- Enemy variety content creation vs. development resources
- Cross-system synergies richness vs. overwhelming complexity
- Story pacing vs. player agency
- RNG excitement vs. frustration prevention

---

## 🚀 NEXT SESSION PRIORITIES

### High Priority (Ready for Deep Dive)
1. **Energy System Mechanics** - Define regeneration, capacity, specialization effects
2. **Enemy Type Catalog** - Create variety, learning curve, weakness systems
3. **Ability Specialization Trees** - Structure paths, define exclusivity, scaling

### Medium Priority (Framework Ready)
1. **Resource Economy Details** - Conversion rates, scarcity curves, storage
2. **POI Encounter Library** - Specific content types and reward structures
3. **Temporal Balance Tuning** - Timer lengths, combat duration, pacing

### Future Sessions
1. **Audio/Visual Concept Development** - Style guide and atmosphere
2. **Technical Planning** - Architecture and implementation strategy
3. **UI/UX Design** - Interface principles and user experience flow

---

## 📊 DESIGN CONFIDENCE LEVELS

### High Confidence ✅
- Core vision and design pillars
- Basic gameplay loop structure
- Combat system framework
- Upgrade philosophy and progression gates

### Medium Confidence 🔄
- Energy system concepts
- Enemy design direction
- Ability categorization
- Cross-system integration approach

### Low Confidence ❓
- Specific balance numbers and tuning
- Resource economy details
- POI content variety and depth
- Technical implementation specifics

### Unknown Territory 📝
- Art direction specifics
- Audio design approach
- UI/UX implementation
- Marketing and distribution strategy

---

**IMPORTANT NOTE**: This is a WORKING document that reflects our collaborative design process. Even areas marked as "established" are still evolving as we refine and discover better approaches through continued design sessions. The goal is to maintain clear vision while staying open to improvements and new insights.

**Design Philosophy**: Every system should support the core vision of meaningful progression that changes how you play, maintain the "runaway train" tension, and create emergent stories through player choice and consequence.

---

*Document will be updated after each collaborative design session to reflect new decisions, refinements, and areas of exploration.*