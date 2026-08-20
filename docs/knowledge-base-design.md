# Knowledge Base Design

## Objective

The Knowledge Hub grounds PathFinder AI in relevant official resources and provides actionable links that students can verify independently.

## Knowledge Categories

### University Programmes

Contains official programme pages for majors referenced by the agent, including examples such as:

- Biomedical Engineering
- Data Science and Analytics
- Business Analytics

### Admissions and Applications

Contains official admissions requirements, application guidance, and application-related resources.

### Financial Aid and Cost

Contains official resources for:

- tuition fees
- tuition grants
- bursaries
- scholarships
- loans
- financial-aid applications
- financial-aid calculators

### Learning Resources

Contains beginner resources used in “try before you choose” plans, including Python and data-science learning materials.

### Overseas Study

Contains official country study portals, scholarship resources, university pages, and visa pages.

## Grounding Strategy

The agent is instructed to:

1. Use direct Knowledge Hub links when available.
2. Prefer exact programme or financial-aid pages over generic homepages.
3. Use an exact `Search: ...` phrase only when a direct link is unavailable.
4. Tell the maintainer which Knowledge Hub section requires an update when a link is missing.
5. Ask students to verify changing information such as fees, deadlines, scholarships, and visa rules.

## Quality Objectives

The Knowledge Hub is designed to improve:

- factual grounding
- actionability
- source transparency
- user trust
- consistency
- resistance to unsupported claims

## Known Retrieval Limitation

A link may exist in the Knowledge Hub but not appear in an answer if the relevant section is not retrieved. This is treated as a retrieval-quality issue rather than solely an instruction-writing issue.

## Maintenance

Resources should be reviewed periodically for:

- broken URLs
- changed programme names
- updated fee structures
- revised financial-aid rules
- changed visa or work regulations
