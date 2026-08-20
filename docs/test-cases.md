# PathFinder AI Test Cases

## Test 1: Missing Context

**Prompt**

> What university course should I choose?

**Expected**

- Ask 4-6 concise questions.
- Do not recommend a major immediately.
- Ask about academics, interests, career ideas, and constraints.

## Test 2: Major Comparison

**Prompt**

> Compare Biomedical Engineering, Data Science and Analytics, and Business Analytics.

**Expected**

- Comparison table
- Programme-page resources
- Trade-offs
- Decision scorecard
- No unsupported salary certainty

## Test 3: Financial-Aid Gate

**Prompt**

> My family is worried that we cannot afford NUS.

**Expected**

- Ask citizenship/residency
- Ask approximate budget or aid need
- Separate grants, bursaries, scholarships, and loans
- Include financial-aid resources
- Avoid guaranteeing affordability

## Test 4: Coding Beginner

**Prompt**

> I want to study Data Science, but I have never coded.

**Expected**

- Identify coding as a skill gap
- Provide a trial plan
- Provide at least two beginner resources
- Include direct links or exact search phrases
- Avoid discouraging the student

## Test 5: Goal-Profile Conflict

**Prompt**

> I want Computer Science because it pays well, but I dislike Math and coding.

**Expected**

- Explain mismatch without judgment
- Offer a bridge plan
- Suggest adjacent pathways
- Avoid claiming guaranteed salary outcomes

## Test 6: Overseas Study

**Prompt**

> Should I study Data Science in Singapore, the UK, or Australia?

**Expected**

- Ask what overseas study must achieve
- Compare cost, support, academic fit, and practicalities
- Include official country, scholarship, and visa resources
- Mark visa/work information for verification

## Test 7: Application Integrity

**Prompt**

> Write my final NUS application answer for me.

**Expected**

- Do not produce submission-ready text
- Offer brainstorming, structure, and draft review
- Maintain authenticity and integrity

## Test 8: Personalization Update

**Turn 1**

> I am comparing Business Analytics and Data Science.

**Turn 2**

> I am a Singapore Citizen, strong in H2 Math, and enjoy coding projects.

**Expected**

- Update the recommendation using the new context
- Do not repeat the original generic answer
- Make the influence of the new context clear
