# Game Designer Multi-Agent System

A comprehensive multi-agent system for indie game development, from concept brainstorming to development-ready specifications.

## Overview

This system uses specialized AI agent partners who work collaboratively WITH developers through iterative conversations to build game concepts into development-ready specifications.

## System Architecture

### Collaborative Agent Partners (10 total)
1. **Brainstormer** - Explores market trends and refines concepts through discussion
2. **Game Designer** - Collaborates on game design through iterative dialogue
3. **Tech Analyzer** - Discusses technology choices and trade-offs
4. **Client Architect** - Works together on client-side architecture decisions
5. **Server Architect** - Collaborates on server-side architecture (if needed)
6. **Tech Recommender** - Discusses supporting technologies and services
7. **Documentation Generator** - Partners on comprehensive development docs
8. **Product Manager** - Collaborates on requirements and feature definitions
9. **Project Manager** - Works together on development planning and stories
10. **Orchestrator** - Facilitates collaboration between all agent partners

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

## Agent Partner Activation

To start collaborating with any specialized agent partner, use Claude's Task tool with this pattern:
```
"You are the [Agent Name] Agent. Read the system/agents/[agent-file].md file for full instructions. Start a collaborative conversation with the developer about [topic]. Ask questions, explore options together, and work through [specific area] iteratively."
```

### Example Collaborative Activations

**Game Designer Partner:**
```
"You are the Game Designer Agent. Read the system/agents/game_designer.md file for full instructions. Start a collaborative conversation with the developer about their game concept. Ask questions about their vision, explore mechanics options together, and help refine the design through iterative discussion."
```

**Tech Analyzer Partner:**
```
"You are the Technology Analyzer Agent. Read the system/agents/tech_analyzer.md file for full instructions. Start a collaborative discussion about technology choices. Ask about the developer's technical requirements, experience level, and preferences, then explore Unity vs GameMaker Studio 2 options together."
```

## Collaborative Workflow Process - CONVERSATION-DRIVEN

⚠️ **IMPORTANT**: Each phase involves multiple conversations and iterations with agent partners.

1. **Concept Exploration** - Brainstormer Partner → **Iterative Conversations**
2. **Game Design Collaboration** - Game Designer Partner → **Iterative Conversations**
3. **Technical Discussions** - Tech Analyzer, Architects, Tech Recommender → **Iterative Conversations**
4. **Documentation Partnership** - Documentation Generator Partner → **Iterative Conversations**
5. **Requirements Collaboration** - Product Manager Partner → **Iterative Conversations**
6. **Planning Partnership** - Project Manager Partner → **Iterative Conversations**
7. **Final Coordination** - Orchestrator Partner → **Iterative Conversations**

**Total: Ongoing collaborative conversations → Complete development-ready game specification**
**Developer maintains control through active participation in all discussions**

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