# Complete Game Design Process Workflow

This workflow coordinates all agents to take a game from initial concept to development-ready specifications.

## Phase 1: Concept Generation
**Agent**: Brainstormer
**Input**: Market research request or refinement of existing concept
**Output**: 5-10 game concepts with market analysis
**Duration**: 1-2 hours research + generation

### Activation Command
```
Use the Task tool with subagent_type "general-purpose" and this prompt:
"You are the Game Brainstormer Agent. [Read the brainstormer.md file for full instructions]. Research current Steam trends, mobile game hits, and emerging gaming technologies. Generate 5-10 unique game concepts that are commercially viable for indie developers. Save your research and concepts to games/[concept-name]/01_concept/ folder."
```

## Phase 2: Concept Development
**Agent**: Game Designer
**Input**: Selected concept from Phase 1
**Output**: Complete game design document
**Duration**: 2-4 hours design work

### Activation Command
```
Use the Task tool with subagent_type "general-purpose" and this prompt:
"You are the Game Designer Agent. [Read the game_designer.md file for full instructions]. Take the selected game concept and develop it into a comprehensive game design including core loops, mechanics, progression, and technical requirements. Save your design work to games/[game-name]/02_design/ folder."
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

## Usage Instructions

1. **Start New Game**: Begin with Phase 1 (Brainstormer Agent)
2. **Select Concept**: Review generated concepts and choose one to develop
3. **Sequential Execution**: Run phases 2-7 in order
4. **Review Points**: Human review recommended after phases 2, 3, and 6
5. **Iteration**: Return to earlier phases if major changes are needed

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