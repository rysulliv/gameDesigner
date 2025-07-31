# Game Designer Multi-Agent System

A comprehensive multi-agent system for indie game development, from concept brainstorming to development-ready specifications.

## Overview

This system uses specialized AI agents to take game concepts through a complete development planning process, producing detailed specifications that a solo indie developer can use to build successful games.

## System Architecture

### Specialized Agents (10 total)
1. **Brainstormer** - Generates game concepts based on market trends
2. **Game Designer** - Develops concepts into complete game designs
3. **Tech Analyzer** - Recommends Unity vs GameMaker Studio 2
4. **Client Architect** - Designs client-side game architecture
5. **Server Architect** - Designs server-side architecture (if needed)
6. **Tech Recommender** - Suggests supporting technologies and services
7. **Documentation Generator** - Creates comprehensive development docs
8. **Product Manager** - Writes PRDs and ensures feature cohesion
9. **Project Manager** - Breaks down work into development stories
10. **Orchestrator** - Coordinates all agents and manages workflow

### File Structure
```
gameDesigner/
├── system/
│   ├── agents/          # 10 specialized agent prompt files
│   ├── templates/       # Standardized document templates
│   └── master_registry.json # Tracks all games and their status
├── games/               # Individual game project folders
├── workflows/           # Process documentation
└── README.md           # This file
```

## Quick Start

### 1. Start a New Game Concept
```
Use Claude's Task tool with this prompt:
"You are the Game Brainstormer Agent. Read the system/agents/brainstormer.md file for full instructions. Research current gaming trends and generate 5-10 unique game concepts suitable for indie development."
```

### 2. Develop Your Chosen Concept
Follow the complete workflow in `workflows/complete_game_design_process.md`

### 3. Review Generated Documentation
Each game project creates:
- Concept and market research
- Complete game design document
- Technical architecture specifications
- Product requirements documents
- Development user stories and timeline

## Individual Game Project Structure

Each game concept gets its own folder:
```
games/[game-name]/
├── 01_concept/
│   ├── initial_brainstorm.md
│   ├── market_research.md
│   └── concept_summary.md
├── 02_design/
│   ├── game_design_document.md
│   ├── core_loop.md
│   ├── mechanics.md
│   └── narrative.md
├── 03_technical/
│   ├── engine_analysis.md
│   ├── client_architecture.md
│   ├── server_architecture.md
│   └── technology_stack.md
├── 04_management/
│   ├── product_requirements.md
│   ├── feature_breakdown.md
│   └── development_stories.md
├── 05_output/
│   ├── final_specification.md
│   └── development_roadmap.md
└── project_status.md
```

## Agent Activation

To use any specialized agent, use Claude's Task tool with this pattern:
```
"You are the [Agent Name] Agent. Read the system/agents/[agent-file].md file for full instructions. [Specific task request]. Save your work to the appropriate game folder."
```

### Example Agent Activations

**Game Designer Agent:**
```
"You are the Game Designer Agent. Read the system/agents/game_designer.md file for full instructions. Take the selected game concept and develop it into comprehensive game design including core loops, mechanics, and progression systems. Save your work to games/[game-name]/02_design/ folder."
```

**Tech Analyzer Agent:**
```
"You are the Technology Analyzer Agent. Read the system/agents/tech_analyzer.md file for full instructions. Analyze the game design requirements and recommend Unity vs GameMaker Studio 2 with detailed reasoning. Save analysis to games/[game-name]/03_technical/ folder."
```

## Complete Workflow Process

1. **Concept Generation** (1-2 hours) - Brainstormer Agent
2. **Game Design** (2-4 hours) - Game Designer Agent  
3. **Technical Planning** (3-5 hours) - Tech Analyzer, Architects, Tech Recommender
4. **Documentation** (1-2 hours) - Documentation Generator Agent
5. **Product Management** (2-3 hours) - Product Manager Agent
6. **Project Planning** (2-4 hours) - Project Manager Agent
7. **Final Review** (1 hour) - Orchestrator Agent

**Total: 12-21 hours of agent work → Complete development-ready game specification**

## Key Features

### For Solo Indie Developers
- Scoped appropriately for small teams
- Focuses on technically feasible solutions
- Considers budget constraints and free/low-cost tools
- Prioritizes rapid development and iteration

### Market-Driven Approach
- Research current gaming trends
- Analyze successful indie games
- Consider platform-specific opportunities
- Validate commercial viability

### Complete Technical Planning
- Engine selection with detailed reasoning
- Client and server architecture design
- Technology stack recommendations
- Performance and scalability considerations

### Development-Ready Output
- Detailed user stories with estimates
- Clear development phases and milestones
- Testing and quality assurance plans
- Launch and marketing considerations

## Master Registry

The `system/master_registry.json` file tracks:
- All game concepts and their current status
- Cross-references between similar games
- Development complexity ratings
- Platform and genre categorization
- Progress tracking across multiple game ideas

## Templates

Standardized templates ensure consistency:
- `game_concept_template.md` - Initial concept documentation
- `prd_template.md` - Product requirements documents
- `technical_spec_template.md` - Technical specifications
- `user_story_template.md` - Development user stories

## Tips for Success

1. **Start Small**: Begin with simpler game concepts to validate the process
2. **Iterate**: Use the system multiple times to refine and improve concepts
3. **Market Research**: Let the Brainstormer Agent do deep market research first
4. **Technical Realism**: Trust the Tech Analyzer's engine recommendations
5. **Scope Management**: Pay attention to complexity ratings and development timelines

## Next Steps

After completing the workflow:
1. Review all generated documentation
2. Validate technical requirements match your skills
3. Set up development environment based on recommendations
4. Begin development using the generated user stories
5. Use the system to explore additional game concepts

---

**Created for indie game developers who want systematic, AI-assisted game design and technical planning.**