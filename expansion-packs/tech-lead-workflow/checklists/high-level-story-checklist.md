# High-Level Story Validation Checklist

This checklist validates that high-level business-focused stories contain sufficient business context and user value clarity for Tech Lead collaborative refinement, without premature technical implementation details.

[[LLM: INITIALIZATION INSTRUCTIONS - HIGH-LEVEL STORY VALIDATION

Before proceeding with this checklist, ensure you have access to:

1. The high-level story document being validated
2. The parent epic or business context
3. Any user journey or business process documentation
4. Business requirements or PRD sections relevant to this story

IMPORTANT: This checklist validates stories BEFORE Tech Lead refinement begins.

VALIDATION PRINCIPLES:

1. Business Value Clarity - User and business value are crystal clear
2. User Focus - Story is written from user perspective with clear outcomes
3. Implementation Agnostic - No premature technical decisions or details
4. Acceptance Criteria - Success is defined from user/business perspective
5. Refinement Ready - Sufficient context for Tech Lead collaborative elaboration

REMEMBER: These are high-level stories that will be technically elaborated through collaboration with the Tech Lead. We're checking for BUSINESS clarity, not technical completeness.]]

## 1. BUSINESS VALUE & PURPOSE CLARITY

[[LLM: Business value must be explicit and compelling. Verify:

1. The story clearly states WHY this matters to users
2. Business benefit is quantifiable or measurable
3. User problem being solved is well-defined
4. Story aligns with overall product/business goals
5. Priority and urgency are justified by business value]]

- [ ] User value is clearly articulated and compelling
- [ ] Business value is explicit and measurable
- [ ] Problem being solved is well-defined
- [ ] Story aligns with broader business goals
- [ ] Priority level is justified by business impact

## 2. USER STORY QUALITY

[[LLM: User stories should follow good agile practices. Check:

1. Follows "As a... I want... So that..." format correctly
2. User type is specific and realistic
3. Desired capability is clear and achievable
4. Benefit/outcome is meaningful to the user
5. Story is sized appropriately (not too big or too small)]]

- [ ] Story follows proper "As a... I want... So that..." format
- [ ] User type is specific and well-defined
- [ ] Desired capability is clear and focused
- [ ] Benefit statement explains meaningful user outcome
- [ ] Story scope is appropriate for agile iteration

## 3. ACCEPTANCE CRITERIA COMPLETENESS

[[LLM: Acceptance criteria define success from user perspective. Ensure:

1. Criteria focus on user-visible behavior and outcomes
2. Success measures are testable and observable
3. Edge cases and error scenarios are considered
4. Criteria avoid technical implementation details
5. Business rules and constraints are captured]]

- [ ] Acceptance criteria focus on user-visible behavior
- [ ] Success criteria are testable and measurable
- [ ] Happy path scenarios are clearly defined
- [ ] Edge cases and error scenarios are addressed
- [ ] Business rules and validation requirements are captured
- [ ] Criteria avoid technical implementation specifics

## 4. USER JOURNEY & CONTEXT

[[LLM: Stories should fit into user workflows and processes. Verify:

1. User journey context is provided
2. Before/after states are clearly described
3. Story fits logically into user workflow
4. Integration with other user processes is considered
5. User experience flow makes sense]]

- [ ] User journey context is clearly described
- [ ] Current state (before story) is documented
- [ ] Future state (after story) is well-defined
- [ ] Story fits logically into user workflow
- [ ] Impact on related user processes is considered

## 5. BUSINESS RULES & CONSTRAINTS

[[LLM: Business logic and constraints drive technical decisions. Check:

1. Business rules are explicitly stated
2. Data validation requirements are clear
3. Workflow and process rules are documented
4. Regulatory or compliance requirements are noted
5. Business constraints and limitations are identified]]

- [ ] Business rules are explicitly documented
- [ ] Data validation requirements are business-focused
- [ ] Workflow and process rules are clear
- [ ] Compliance or regulatory requirements are noted
- [ ] Business constraints and limitations are identified

## 6. DEPENDENCY & ASSUMPTION CLARITY

[[LLM: Dependencies and assumptions affect implementation approach. Ensure:

1. Dependencies on other stories/features are explicit
2. External system dependencies are identified
3. Data dependencies are noted
4. Assumptions about user behavior are stated
5. Business process assumptions are documented]]

- [ ] Dependencies on other stories are explicitly stated
- [ ] External system or data dependencies are identified
- [ ] User behavior assumptions are documented
- [ ] Business process assumptions are clear
- [ ] Organizational or resource dependencies are noted

## 7. REFINEMENT READINESS

[[LLM: Story should provide sufficient context for Tech Lead collaboration. Verify:

1. Business context is sufficient for technical elaboration
2. Questions for Tech Lead are identified
3. Areas requiring technical input are noted
4. Implementation flexibility is appropriate
5. Story is ready for collaborative technical design]]

- [ ] Sufficient business context for technical elaboration
- [ ] Key questions for Tech Lead are identified
- [ ] Areas requiring technical expertise are noted
- [ ] Appropriate flexibility for implementation approach
- [ ] Story is self-contained enough for refinement session

## 8. SUCCESS METRICS & MEASUREMENT

[[LLM: Success should be measurable from business perspective. Check:

1. User success metrics are defined
2. Business success metrics are identified
3. Measurement approach is feasible
4. Success indicators are observable
5. Metrics align with business value proposition]]

- [ ] User success metrics are clearly defined
- [ ] Business success metrics are identified
- [ ] Measurement approach is practical and feasible
- [ ] Success indicators are observable and trackable
- [ ] Metrics directly support stated business value

## 9. IMPLEMENTATION NEUTRALITY

[[LLM: High-level stories should avoid premature technical decisions. Ensure:

1. No specific technologies are mandated unnecessarily
2. Technical approach is left open for Tech Lead input
3. Focus is on WHAT and WHY, not HOW
4. Implementation details are appropriately deferred
5. Story doesn't constrain technical creativity]]

- [ ] Story avoids unnecessary technology mandates
- [ ] Technical approach is left open for collaborative design
- [ ] Focus is on business outcomes, not implementation details
- [ ] Technical constraints are business-driven, not arbitrary
- [ ] Implementation creativity is preserved for Tech Lead refinement

## VALIDATION RESULT

[[LLM: HIGH-LEVEL STORY VALIDATION REPORT

Generate a business-focused validation report:

1. Business Readiness Summary

   - Story readiness: READY FOR REFINEMENT / NEEDS BUSINESS CLARIFICATION / BLOCKED
   - Business value clarity (1-10)
   - User value clarity (1-10)
   - Major business gaps identified

2. Fill in the validation table with:

   - PASS: Business requirements clearly met
   - PARTIAL: Some business gaps but workable for refinement
   - FAIL: Critical business information missing

3. Specific Business Issues (if any)

   - List concrete business problems to clarify
   - Suggest specific business improvements
   - Identify any business dependencies or blockers

4. Tech Lead Refinement Readiness
   - Is business context sufficient for technical elaboration?
   - What business questions need answers before refinement?
   - Are business constraints and requirements clear?
   - Is user value compelling enough to justify technical effort?

Focus on business clarity and user value - technical implementation will be collaboratively designed with the Tech Lead.]]

| Category                          | Status | Issues |
| --------------------------------- | ------ | ------ |
| 1. Business Value & Purpose       | _TBD_  |        |
| 2. User Story Quality             | _TBD_  |        |
| 3. Acceptance Criteria            | _TBD_  |        |
| 4. User Journey & Context         | _TBD_  |        |
| 5. Business Rules & Constraints   | _TBD_  |        |
| 6. Dependency & Assumption        | _TBD_  |        |
| 7. Refinement Readiness           | _TBD_  |        |
| 8. Success Metrics               | _TBD_  |        |
| 9. Implementation Neutrality      | _TBD_  |        |

**Final Assessment:**

- **READY FOR REFINEMENT**: Story provides sufficient business context for Tech Lead collaborative elaboration
- **NEEDS BUSINESS CLARIFICATION**: Story requires business updates before refinement (see issues)
- **BLOCKED**: External business information or decisions required (specify what information)