# PathFinder AI

> An evaluation-driven university decision-support agent built with Microsoft Copilot Studio.

PathFinder AI helps pre-university students compare majors, understand university affordability, explore career pathways, and access official programme, financial-aid, and overseas-study resources.

The project focuses on AI behaviour design, personalization, knowledge grounding, instruction-following, uncertainty calibration, and systematic response evaluation.

## Demo

- **Demo video:** https://drive.google.com/file/d/1t1Jq0oBb0ENCoeTG3d9xN1xllomvX0o7/view?usp=drive_link
- **Pitch deck:** assets/pathfinder-ai-deck.pdf
- **Evaluation report:** docs/evaluation-report.md
- **Test suite:** docs/test-cases.md

### Example Scenario

> I want to study at NUS, but my family is worried we cannot afford it. I am choosing between Business Analytics and Data Science. Which one is safer financially?

PathFinder AI is expected to:

- identify both the academic and financial dimensions
- ask for citizenship or residency when unknown
- compare the programmes using a structured table
- distinguish financial safety from maximum salary potential
- provide a decision scorecard
- include official programme and financial-aid resources
- avoid guaranteeing affordability, employment, or salary

assets/demo-financial-aid.png

## Problem

Students face high-stakes decisions when choosing:

- university programmes
- local or overseas universities
- career pathways
- financial-aid options
- scholarships and loans

Available information is often fragmented across programme pages, admission portals, government websites, and informal advice.

General-purpose AI assistants may also produce answers that are:

- too generic
- insufficiently personalized
- overly confident
- weakly sourced
- difficult to act on

PathFinder AI was designed to reduce these quality gaps.

## Target Users

- Junior College students
- Polytechnic students
- pre-university students comparing majors
- students with affordability concerns
- students comparing local and overseas pathways
- students who are undecided about university or career direction

## Solution

PathFinder AI combines:

- student-context collection
- structured decision support
- programme comparison
- career-pathway exploration
- affordability and financial-aid guidance
- skill-gap diagnosis
- official resource retrieval
- backup pathway planning

Instead of only answering a question, the agent helps the student understand the decision, compare trade-offs, test possible pathways, and take practical next steps.

## Core Features

### 1. Personalized Guidance

The agent considers relevant context such as:

- subjects and grades
- academic strengths and weaknesses
- interests and projects
- intended careers
- learning preferences
- citizenship or residency
- budget and financial-aid needs
- local or overseas study preferences

If critical context is missing, the agent asks a small number of targeted questions before making a recommendation.

### 2. Structured Decision Support

Responses may include:

- side-by-side comparison tables
- decision scorecards
- trade-off analysis
- risks and mitigation
- skill-gap diagnosis
- Plan A, Plan B, and Plan C pathways
- one-week or two-week exploration plans

### 3. Financial-Aid Reasoning

When affordability is mentioned, the agent is instructed to ask for relevant missing information before giving specific guidance.

This may include:

- citizenship or residency
- approximate family budget or financial-aid need
- willingness to consider bursaries, scholarships, loans, or work-study

The agent then separates:

- tuition grants or subsidies
- bursaries
- scholarships
- loans
- accommodation
- transport
- living and learning expenses

### 4. Knowledge-Grounded Guidance

The curated Knowledge Hub includes:

- official university programme pages
- admissions information
- tuition and financial-aid pages
- scholarship resources
- beginner learning resources
- official overseas-study portals
- visa and government resources

The agent is instructed to use exact Knowledge Hub links when available. If a direct link is unavailable, the agent provides an exact search phrase and identifies the section that should be updated.

### 5. Application Integrity

The agent can help students with:

- brainstorming
- response structure
- reflection prompts
- CV organization
- draft review
- application timeline planning

The agent is instructed not to:

- fabricate achievements
- exaggerate impact
- ghostwrite submission-ready essays
- encourage cheating or unethical shortcuts

## System Architecture

```text
Student Query
      |
      v
Student Context and Constraints
      |
      v
PathFinder AI System Instructions
      |
      +----------------------+
      |                      |
      v                      v
Decision Framework      Curated Knowledge Hub
      |                      |
      +----------+-----------+
                 |
                 v
Grounded and Structured Response
                 |
                 v
Comparison + Resources + Next Steps
