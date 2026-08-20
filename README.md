# PathFinder AI

> An evaluation-driven university decision-support agent built with Microsoft Copilot Studio.

PathFinder AI helps pre-university students compare majors, understand university affordability, explore career pathways, and access official programme and financial-aid resources.

This project focuses on AI behaviour design, personalization, knowledge grounding, instruction-following, and systematic response evaluation.

## Project Overview

University decisions involve more than identifying a popular course. Students must consider:

- academic interests and readiness
- programme workload and prerequisites
- career flexibility
- tuition and living costs
- citizenship-dependent financial aid
- local and overseas alternatives

General-purpose AI assistants can produce helpful information, but their answers may be generic, overly confident, poorly sourced, or insufficiently personalized.

PathFinder AI was designed to address these quality gaps.

## Target Users

- Junior College and Polytechnic students
- Pre-university students comparing majors
- Students with financial-aid concerns
- Students comparing local and overseas pathways
- Students who are undecided about university and career direction

## Core Capabilities

### Personalized decision support

The agent considers relevant context such as:

- subjects and grades
- interests and projects
- intended careers
- learning preferences
- citizenship or residency
- budget and financial-aid needs

### Structured comparisons

Responses may include:

- comparison tables
- decision scorecards
- trade-off analysis
- skill-gap diagnosis
- Plan A, Plan B, and Plan C pathways
- short exploration plans

### Financial-aid reasoning

When affordability is mentioned, the agent asks for relevant missing information before giving specific guidance, including:

- citizenship or residency
- approximate budget or aid need
- willingness to consider bursaries, scholarships, loans, or work-study

### Knowledge-grounded guidance

The curated Knowledge Hub contains:

- official university programme pages
- admissions information
- tuition and financial-aid resources
- beginner learning resources
- overseas study portals
- official visa and scholarship resources

### Application integrity

The agent supports brainstorming, structure, draft review, and reflection. It is instructed not to fabricate achievements or produce submission-ready application essays.

## Why This Project Is Relevant to AI Quality Evaluation

This project was developed through an iterative evaluation cycle:

1. Define expected agent behaviour
2. Construct realistic test prompts
3. Review actual responses
4. Identify instruction-following and grounding failures
5. Revise system instructions and knowledge resources
6. Retest for consistency and usefulness
7. Document remaining limitations

Examples of issues identified during testing included:

- failing to ask citizenship before financial-aid guidance
- recommending resources without direct links
- mixing programme and financial-aid resources
- making overly confident career or affordability claims
- giving recommendations before collecting critical context

These failures were converted into explicit evaluation criteria and instruction updates.

## Example: Major and Affordability Decision

**User scenario**

> I want to study at NUS, but my family is worried we cannot afford it. I am choosing between Business Analytics and Data Science. Which one is safer financially?

**Expected agent behaviour**

- summarize the student’s concern
- ask citizenship or residency if unknown
- compare both majors across workload and career flexibility
- distinguish academic risk from salary potential
- provide financial-aid resources
- provide official programme links
- avoid guaranteeing affordability or employment

See the full evaluation in docs/evaluation-report.md.

## Repository Structure

```text
docs/              Agent design and evaluation documentation
prompts/           Agent system instructions
knowledge-base/    Curated grounding resources
evaluation/        Evaluation matrix and test cases
assets/            Screenshots, deck, and demo information
