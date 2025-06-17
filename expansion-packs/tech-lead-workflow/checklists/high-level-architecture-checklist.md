# High-Level Architecture Validation Checklist

This checklist validates strategic architectural decisions without diving into implementation details. The Enhanced Architect uses this to ensure framework choices, patterns, and quality attributes are sound before handing off to Tech Lead for implementation elaboration.

[[LLM: INITIALIZATION INSTRUCTIONS - REQUIRED ARTIFACTS

Before proceeding with this checklist, ensure you have access to:

1. high-level-architecture.md - The strategic architecture document
2. prd.md - Product Requirements Document for business alignment
3. framework-selection.md - Technology selection rationale (if exists)
4. quality-attributes.md - Non-functional requirements (if exists)

IMPORTANT: This checklist focuses on STRATEGIC decisions only. Implementation details will be handled by the Tech Lead during collaborative story refinement.

VALIDATION APPROACH:
For each section, you must:

1. Strategic Analysis - Focus on framework and pattern choices, not implementation
2. Business Alignment - Ensure architectural patterns support business goals
3. Quality Focus - Validate quality attributes and constraints are addressed
4. Handoff Preparation - Ensure sufficient strategic context for Tech Lead elaboration

EXECUTION MODE:
Ask the user if they want to work through the checklist:

- Section by section (interactive mode) - Review each section, present findings, get confirmation before proceeding
- All at once (strategic assessment mode) - Complete full strategic analysis and present comprehensive report at end]]

## 1. STRATEGIC REQUIREMENTS ALIGNMENT

[[LLM: Focus on high-level business alignment, not detailed functional requirements. Validate that the architectural approach supports the business vision and user outcomes.]]

### 1.1 Business Goals Alignment

- [ ] Architecture supports core business objectives
- [ ] Technology choices align with organizational strategy
- [ ] Architecture patterns support expected user journeys
- [ ] Strategic technical decisions support business model
- [ ] Architectural approach enables business scalability

### 1.2 Quality Attributes Prioritization

- [ ] Critical quality attributes are identified and prioritized
- [ ] Performance targets are realistic and business-driven
- [ ] Scalability requirements align with growth projections
- [ ] Security requirements match business risk profile
- [ ] Reliability needs support business operations

### 1.3 Strategic Constraints Recognition

- [ ] Organizational constraints are acknowledged
- [ ] Budget and timeline constraints influence technology choices
- [ ] Team capability constraints are considered
- [ ] Existing system constraints are identified
- [ ] Compliance requirements are recognized at strategic level

## 2. FRAMEWORK & TECHNOLOGY STRATEGY

[[LLM: Validate strategic technology decisions and framework choices. Focus on WHY technologies were chosen, not HOW they will be implemented.]]

### 2.1 Technology Selection Rationale

- [ ] Primary technology stack choices are justified
- [ ] Framework selections support quality attributes
- [ ] Technology decisions consider team expertise
- [ ] Alternatives were evaluated with clear criteria
- [ ] Technology choices support long-term maintainability

### 2.2 Architectural Pattern Coherence

- [ ] Primary architectural pattern is clearly defined
- [ ] Pattern choice supports quality requirements
- [ ] Pattern aligns with team capabilities
- [ ] Pattern supports expected system evolution
- [ ] Pattern choice is consistently applied

### 2.3 Integration Strategy

- [ ] External system integration approach is defined
- [ ] Third-party service strategy is established
- [ ] Data integration patterns are identified
- [ ] API strategy supports business requirements
- [ ] Integration approach supports scalability

## 3. SYSTEM BOUNDARIES & SCOPE

[[LLM: Validate that system boundaries are clearly defined and scope is appropriate for the business context.]]

### 3.1 System Scope Definition

- [ ] What the system does is clearly defined
- [ ] What the system does NOT do is explicitly stated
- [ ] System boundaries are appropriate for business goals
- [ ] Scope aligns with available resources
- [ ] Future expansion possibilities are considered

### 3.2 Stakeholder Context

- [ ] Primary users and their needs are identified
- [ ] Secondary stakeholders are acknowledged
- [ ] Integration touchpoints are mapped
- [ ] Operational stakeholders are considered
- [ ] Business stakeholder needs are addressed

### 3.3 Environmental Considerations

- [ ] Deployment environment strategy is defined
- [ ] Operational environment constraints are acknowledged
- [ ] Development environment approach is established
- [ ] Security environment requirements are identified
- [ ] Compliance environment needs are recognized

## 4. STRATEGIC QUALITY ATTRIBUTES

[[LLM: Focus on quality attributes as architectural drivers, not implementation specifics. Validate that the architecture supports the required quality characteristics.]]

### 4.1 Performance Strategy

- [ ] Performance requirements are realistic and measurable
- [ ] Performance approach aligns with user expectations
- [ ] Performance strategy supports business operations
- [ ] Performance targets consider cost implications
- [ ] Performance approach enables monitoring

### 4.2 Scalability Approach

- [ ] Scalability requirements match business projections
- [ ] Scaling approach (horizontal/vertical) is defined
- [ ] Scalability strategy considers cost implications
- [ ] Scaling approach aligns with operational capabilities
- [ ] Scalability supports user growth patterns

### 4.3 Security & Compliance Framework

- [ ] Security approach matches business risk profile
- [ ] Compliance requirements are identified and addressed
- [ ] Security strategy enables business operations
- [ ] Privacy requirements are acknowledged
- [ ] Security approach supports user trust

### 4.4 Maintainability & Evolution

- [ ] Architecture supports expected change patterns
- [ ] Maintainability approach matches team capabilities
- [ ] Evolution strategy supports business growth
- [ ] Technical debt management approach is considered
- [ ] Architecture enables continuous improvement

## 5. STRATEGIC RISK ASSESSMENT

[[LLM: Focus on strategic and architectural risks, not implementation risks. Consider business impact and mitigation approaches.]]

### 5.1 Technology Risk Management

- [ ] Technology adoption risks are identified
- [ ] Vendor lock-in risks are acknowledged
- [ ] Technology obsolescence risks are considered
- [ ] Team learning curve risks are assessed
- [ ] Technology maturity risks are evaluated

### 5.2 Architectural Risk Mitigation

- [ ] Single points of failure are identified
- [ ] Critical dependency risks are acknowledged
- [ ] Scalability bottleneck risks are considered
- [ ] Integration failure risks are assessed
- [ ] Data loss/corruption risks are identified

### 5.3 Business Continuity Considerations

- [ ] Disaster recovery approach is defined at strategic level
- [ ] Business continuity requirements are identified
- [ ] Operational resilience approach is established
- [ ] Critical business function protection is considered
- [ ] Recovery objectives align with business needs

## 6. HANDOFF READINESS FOR TECH LEAD

[[LLM: Validate that sufficient strategic context exists for Tech Lead to begin collaborative technical elaboration.]]

### 6.1 Strategic Context Completeness

- [ ] Framework decisions provide clear guidance
- [ ] Quality attributes give implementation direction
- [ ] Technology choices enable detailed design
- [ ] Architectural patterns guide component design
- [ ] Business context informs technical decisions

### 6.2 Decision Rationale Documentation

- [ ] Key architectural decisions are documented
- [ ] Technology choice rationale is clear
- [ ] Trade-offs are explicitly acknowledged
- [ ] Assumptions are stated clearly
- [ ] Constraints are well-documented

### 6.3 Implementation Boundary Definition

- [ ] What needs Tech Lead elaboration is clear
- [ ] What should NOT be changed is identified
- [ ] Flexibility areas are explicitly noted
- [ ] Non-negotiable constraints are highlighted
- [ ] Collaborative decision areas are marked

## 7. ORGANIZATIONAL ALIGNMENT

[[LLM: Validate that the architecture aligns with organizational capabilities and constraints.]]

### 7.1 Team Capability Alignment

- [ ] Architecture matches current team skills
- [ ] Learning requirements are reasonable
- [ ] Architecture enables team productivity
- [ ] Skill development path is considered
- [ ] Team structure supports architecture

### 7.2 Organizational Process Alignment

- [ ] Architecture supports development processes
- [ ] Deployment approach aligns with DevOps capabilities
- [ ] Testing strategy matches organizational maturity
- [ ] Documentation approach fits team practices
- [ ] Quality processes are supported

### 7.3 Resource & Timeline Realism

- [ ] Architecture scope fits available timeline
- [ ] Resource requirements are realistic
- [ ] Dependencies on external teams are identified
- [ ] Critical path considerations are acknowledged
- [ ] Risk mitigation time is included

[[LLM: STRATEGIC VALIDATION REPORT GENERATION

Now that you've completed the strategic checklist, generate a focused validation report that includes:

1. Strategic Readiness Summary
   - Overall strategic architecture soundness (High/Medium/Low)
   - Critical strategic gaps identified
   - Key strengths of the strategic approach
   - Readiness for Tech Lead collaborative elaboration

2. Framework & Technology Assessment
   - Technology selection appropriateness
   - Framework choice alignment with requirements
   - Strategic technology risks and mitigations

3. Quality Attributes Validation
   - Quality attribute completeness and realism
   - Strategic quality approach soundness
   - Quality-driven architectural decisions

4. Business Alignment Verification
   - Business goal support assessment
   - Stakeholder needs alignment
   - Organizational capability match

5. Tech Lead Handoff Readiness
   - Sufficiency of strategic context for implementation elaboration
   - Clear boundaries for collaborative technical design
   - Areas requiring Tech Lead input and collaboration

6. Strategic Recommendations
   - Must-address strategic gaps before Tech Lead handoff
   - Should-address items for better strategic foundation
   - Collaborative elaboration focus areas

After presenting the report, ask the user if they would like detailed analysis of any specific strategic area or preparation for Tech Lead handoff.]]