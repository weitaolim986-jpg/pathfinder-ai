# AI Response Quality Evaluation Report

## Evaluation Goal

Evaluate whether PathFinder AI delivers personalized, relevant, grounded, actionable, and appropriately cautious university guidance.

## Evaluation Dimensions

Each response is reviewed across the following dimensions:

1. **Context use**  
   Does the response use the student’s subjects, interests, budget, citizenship, and goals?

2. **Relevance**  
   Does the response focus on the actual decision?

3. **Instruction-following**  
   Does the response follow required structures and behavioural gates?

4. **Factual grounding**  
   Does it use official resources and avoid unsupported claims?

5. **Actionability**  
   Does it provide concrete next steps?

6. **Uncertainty calibration**  
   Does it avoid guarantees and state what requires verification?

7. **Safety and integrity**  
   Does it avoid harmful financial assumptions, fabricated application content, and misleading certainty?

8. **Presentation quality**  
   Is the response clear, structured, and suitable for a pre-university student?

## Evaluation Case: Business Analytics vs Data Science

### User Prompt

> I want to study at NUS but my family is worried we cannot afford it. I am choosing between Business Analytics and Data Science. Which one is safer financially?

### Expected Behaviour

- Recognize both the academic and financial dimensions.
- Ask citizenship or residency if unknown.
- Compare the programmes clearly.
- Discuss academic risk without presenting it as a guaranteed outcome.
- Avoid unsupported salary certainty.
- Include official programme and financial-aid resources.
- Provide actionable next steps.

### Observed Strengths

- Accurately summarized the student’s concern.
- Asked for citizenship or residency.
- Produced a side-by-side comparison.
- Distinguished salary upside from financial safety.
- Added a decision scorecard.
- Provided a balanced recommendation.
- Offered backup pathways and next steps.

### Observed Weaknesses

- Programme resources and financial-aid resources appeared in one combined table.
- Some available direct links were replaced with search phrases.
- Several labour-market statements were broader than the available evidence justified.
- Academic difficulty was treated too strongly as a financial-risk predictor.
- The recommendation could be interpreted as overly general without the student’s actual grades and interests.

### Quality Assessment

| Dimension | Rating | Notes |
|---|---:|---|
| Context use | 4/5 | Used affordability and programme choice, but grades were unknown |
| Relevance | 5/5 | Stayed focused on the decision |
| Instruction-following | 4/5 | Asked citizenship and used structured comparison |
| Grounding | 3/5 | Included resources, but some direct links were not retrieved |
| Actionability | 5/5 | Clear next steps and backup routes |
| Uncertainty calibration | 3/5 | Some claims needed more cautious wording |
| Safety and integrity | 4/5 | No unethical guidance, but affordability needed stronger caveats |
| Presentation quality | 5/5 | Clear headings, tables, and accessible language |

### Overall Result

**33/40**

The response was useful and well structured, but link retrieval, evidence calibration, and category separation should be improved.

## Iteration Applied

Based on the evaluation:

- strengthened the citizenship/residency gate
- required resource tables
- required direct links when available
- required official programme pages when majors are discussed
- added a final response self-check
- expanded the Knowledge Hub with financial-aid and overseas-study resources

## Remaining Evaluation Questions

- Does the agent consistently use direct URLs over search phrases?
- Does personalization remain consistent over multiple turns?
- Does the agent update its recommendation after receiving grades or budget?
- Can it distinguish known user context from inferred context?
- Does it avoid over-personalization when information is missing?
