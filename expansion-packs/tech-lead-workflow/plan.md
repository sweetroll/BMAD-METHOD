# Tech Lead Workflow Extension Pack Plan

## Overview

- **Pack Name**: tech-lead-workflow
- **Display Name**: Tech Lead Workflow Extension
- **Pack Type**: Agent Enhancement Extension (No orchestrator required)
- **Description**: Rebalances BMAD workflow with high-level architecture, high-level stories, and collaborative just-in-time technical elaboration
- **Target Domain**: Agile software development teams
- **Author**: BMAD Community

## Problem Statement

Current BMAD workflow forces premature technical detail at wrong stages:
- Architects pressured into implementation specifics too early
- Scrum Masters create technically detailed stories before collaborative design
- Developers receive pre-made technical decisions without collaborative input
- Missing just-in-time technical elaboration that happens in real agile teams

This pack introduces a Tech Lead persona that bridges high-level architecture with implementation through collaborative technical refinement.

## Target Users

Development teams who want:
- Natural agile workflow timing for technical decisions
- Collaborative technical design between leads and developers
- High-level architecture without premature implementation details
- Business-focused user stories that get technically elaborated just-in-time

## Components to Create

### Agents

- [ ] `tech-lead-workflow-orchestrator` - **CREATED**: Lightweight workflow documentation tool
  - **Purpose**: Process guidance, status tracking, handoff documentation
  - **Functionality**: Documents story status, suggests next agent, tracks handoffs
  - **Approach**: Manual control - no automation, just better organization
  - **Agent Name**: Tech Lead Workflow Guide - Helps organize and track workflow process
- [ ] `architect` - **OVERRIDES CORE**: Strategic high-level architecture without implementation details
  - Tasks used: create-doc, create-deep-research-prompt, document-project
  - Templates used: high-level-architecture-tmpl, framework-selection-tmpl, quality-attributes-tmpl
  - Data required: technical-preferences
  - **Override Strategy**: Replaces core architect.md with high-level focused version
- [ ] `sm` - **OVERRIDES CORE**: High-level business-focused story creation
  - Tasks used: create-doc, advanced-elicitation, high-level-story-creation
  - Templates used: high-level-story-tmpl, story-acceptance-criteria-tmpl
  - Data required: bmad-kb
  - **Override Strategy**: Replaces core sm.md with business-focused version
- [ ] `tech-lead` - **CREATED**: Collaborative technical refinement and implementation planning
  - Tasks used: story-refinement, technical-decision-capture, implementation-planning, create-doc
  - Templates used: story-refinement-tmpl, tech-decision-tmpl, implementation-plan-tmpl
  - Data required: technical-preferences
  - **Agent Name**: Beryl - Collaborative Tech Lead specializing in just-in-time technical elaboration

### Tasks

- [ ] `story-enhancement.md` - **CREATED**: Enhance high-level stories with developer steps and status management (used by: tech-lead)
- [ ] `technical-decision-capture.md` - **CREATED**: Document implementation decisions and rationale (used by: tech-lead)
- [ ] `implementation-planning.md` - **CREATED**: Bridge user stories to actionable dev tasks (used by: tech-lead)
- [ ] `high-level-story-creation.md` - **CREATED**: Business-focused story creation process (used by: enhanced-scrum-master)

### Templates

- [ ] `high-level-story-tmpl.md` - **CREATED**: Business-focused user stories without technical details (used by: enhanced-scrum-master)
- [ ] `story-acceptance-criteria-tmpl.md` - **CREATED**: Clear acceptance criteria focused on user value (used by: enhanced-scrum-master)
- [ ] `tech-decision-tmpl.md` - **CREATED**: Technical decision and rationale documentation (used by: tech-lead)
- [ ] `implementation-plan-tmpl.md` - **CREATED**: Actionable development tasks with technical context (used by: tech-lead)
- [ ] `tech-lead-knowledge-base-tmpl.md` - **CREATED**: Capture technical insights and patterns for future stories (used by: tech-lead)

### Checklists

- [ ] `high-level-architecture-checklist.md` - **CREATED**: Validates strategic architecture without premature details
- [ ] `high-level-story-checklist.md` - **CREATED**: Validates business-focused stories for Tech Lead refinement readiness
- [ ] `story-refinement-checklist.md` - **CREATED**: Ensures complete collaborative technical elaboration

### Data Files Required from User

Users must add these files to `bmad-core/data/`:

- [ ] `technical-preferences.md` - **ALREADY EXISTS**: Team's technology preferences and constraints
  - Format: Markdown with structured sections
  - Purpose: Guide framework and technology choices
  - Example: Framework preferences, coding standards, tooling choices

*Note: This pack primarily uses existing BMAD data files and enhances workflow timing rather than requiring new domain-specific data.*

## Workflow Overview

1. **High-Level Architecture**: Enhanced Architect creates strategic framework decisions and quality attributes
2. **High-Level Stories**: Enhanced Scrum Master creates business-focused user stories (status: HIGH_LEVEL)
3. **Manual Review Gate 1**: Product Owner manually updates status to APPROVED_FOR_REFINEMENT
4. **Collaborative Refinement**: Tech Lead works with Developer to elaborate technical implementation and updates status to PENDING_DEVELOPMENT_APPROVAL
5. **Manual Review Gate 2**: Product Owner manually updates status to APPROVED (for BMAD dev agent compatibility)
6. **Implementation**: BMAD dev agent executes with maintained technical context and documented decisions

## Integration Points

- Depends on core agents: architect (enhanced), sm (enhanced), dev (existing)
- Extends teams: team-all.yml, team-fullstack.yml with new workflow option
- Enhances existing workflow: Provides alternative to current direct architect→dev flow

## Success Criteria

- [ ] All components created and cross-referenced
- [ ] No orphaned task/template references  
- [ ] Enhanced agents maintain backward compatibility
- [ ] Orchestrator provides clear workflow guidance
- [ ] README includes migration from current workflow
- [ ] Just-in-time technical elaboration works smoothly
- [ ] Collaborative refinement templates support developer input

## User Approval

- [ ] Plan reviewed by user
- [ ] Approval to proceed with implementation

---

**Next Steps**: Once approved, proceed with Phase 3 implementation starting with the orchestrator agent.