# Collaborative Game Design Process Workflow

This workflow coordinates specialized agent partners who work WITH developers through iterative conversations to build games collaboratively.

## Phase 1: Concept Exploration
**Agent Partner**: Brainstormer
**Collaborative Goal**: Explore market opportunities and refine game concepts together
**Duration**: Multiple conversations until concept is refined

### Conversation Approach
The Brainstormer Agent will:
- Ask about your gaming interests and development goals
- Share market trends and opportunities for discussion
- Suggest multiple concept directions based on your interests
- Help refine ideas through iterative dialogue
- Question assumptions to strengthen concepts

### Activation Approach
```
"You are the Game Brainstormer Agent. Read the brainstormer.md file for full instructions. Start a collaborative conversation with the developer to explore game concepts. Ask about their interests, share market insights, and work together to refine ideas through discussion."
```

## Phase 2: Game Design Collaboration
**Agent Partner**: Game Designer
**Collaborative Goal**: Work together to build comprehensive game design through dialogue
**Duration**: Multiple conversations exploring mechanics, loops, and systems

### Conversation Approach
The Game Designer Agent will:
- Ask questions about your vision and player experience goals
- Present multiple design approaches for each system
- Explore mechanics options and their implications
- Help identify potential design challenges early
- Iterate on ideas based on your feedback

### Activation Approach
```
"You are the Game Designer Agent. Read the game_designer.md file for full instructions. Start a collaborative conversation with the developer about their game concept. Ask questions about their vision, explore mechanics options together, and help refine the design through iterative discussion."
```

## Phase 3: Technical Analysis
**Agents**: Tech Analyzer, Client Architect, Server Architect, Tech Recommender
**Input**: Game design from Phase 2
**Output**: Complete technical specification
**Duration**: 3-5 hours architecture work

### Activation Commands
```
Tech Analyzer:
"You are the Technology Analyzer Agent. [Read the tech_analyzer.md file]. Analyze the game design and recommend Unity vs GameMaker Studio 2. Save analysis to games/[game-name]/03_technical/ folder."

Client Architect:
"You are the Client Architecture Agent. [Read the client_architect.md file]. Design the client-side architecture based on the game requirements. Save architectural designs to games/[game-name]/03_technical/ folder."

Server Architect:
"You are the Server Architecture Agent. [Read the server_architect.md file]. Determine server needs and design server architecture if required. Save designs to games/[game-name]/03_technical/ folder."

Tech Recommender:
"You are the Technology Recommender Agent. [Read the tech_recommender.md file]. Recommend supporting technologies and services for the game. Save recommendations to games/[game-name]/03_technical/ folder."
```

## Phase 4: Documentation
**Agent**: Documentation Generator
**Input**: All previous phase outputs
**Output**: Comprehensive development documentation
**Duration**: 1-2 hours synthesis

### Activation Command
```
Use the Task tool with subagent_type "general-purpose" and this prompt:
"You are the Documentation Generator Agent. [Read the documentation_generator.md file]. Synthesize all previous agent work into comprehensive development documentation. Create TDD, GDD, roadmap, and specifications. Save all documentation to games/[game-name]/05_output/ folder."
```

## Phase 5: Product Management
**Agent**: Product Manager
**Input**: Game design and technical specs
**Output**: PRDs for game and major features
**Duration**: 2-3 hours requirements work

### Activation Command
```
Use the Task tool with subagent_type "general-purpose" and this prompt:
"You are the Product Manager Agent. [Read the product_manager.md file]. Create comprehensive PRDs for the overall game and major features. Ensure all systems connect logically. Save all PRDs to games/[game-name]/04_management/ folder."
```

## Phase 6: Project Planning
**Agent**: Project Manager
**Input**: PRDs and technical specifications
**Output**: Development stories and timeline
**Duration**: 2-4 hours planning work

### Activation Command
```
Use the Task tool with subagent_type "general-purpose" and this prompt:
"You are the Project Manager Agent. [Read the project_manager.md file]. Convert PRDs into specific development stories with estimates and dependencies. Create logical development phases. Save development stories to games/[game-name]/04_management/ folder."
```

## Phase 7: Final Review
**Agent**: Orchestrator
**Input**: All deliverables
**Output**: Quality-checked, complete project package
**Duration**: 1 hour review and refinement

### Activation Command
```
Use the Task tool with subagent_type "general-purpose" and this prompt:
"You are the Orchestrator Agent. [Read the orchestrator.md file]. Review all deliverables for completeness and consistency. Ensure the indie developer has clear next actions and complete documentation. Update the master registry. Save coordination notes to games/[game-name]/ root folder."
```

## Total Timeline
**Estimated Duration**: 12-21 hours of agent work
**Human Decisions Required**: Concept selection, design approval, technical preferences
**Output**: Complete development-ready game specification

## Usage Instructions - HUMAN-GUIDED WORKFLOW

⚠️ **IMPORTANT**: Execute ONE phase at a time with human review and approval between each step.

1. **Start New Game**: Begin with Phase 1 (Brainstormer Agent)
2. **Select Concept**: Review generated concepts and choose one to develop
3. **Step-by-Step Execution**: 
   - Execute ONE phase only
   - Wait for human review and feedback
   - Make refinements based on feedback
   - Get explicit approval before proceeding to next phase
4. **Required Review Points**: Human review and approval required after EVERY phase
5. **Iteration**: Return to earlier phases if major changes are needed

### Agent Activation Protocol
- Agents should ONLY be activated when explicitly requested by the human
- No automatic progression to next phase
- Each agent waits for specific activation command
- Human maintains control over workflow progression

## File Organization

Each game follows this structure:
```
games/[game-name]/
├── 01_concept/          # Brainstorming and market research
├── 02_design/           # Game design documents
├── 03_technical/        # Technical specifications
├── 04_management/       # PRDs and project planning
├── 05_output/           # Final documentation
└── project_status.md    # Overall project tracking
```

## Master Registry Updates

After each phase, the Orchestrator agent should update the master registry with:
- Current project status
- Completion of phase milestones
- Key decisions and recommendations
- Cross-references to other similar games