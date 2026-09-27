# AI Evaluation Rubric

A consistent framework for assessing AI-generated responses.

## Scoring

Each dimension is scored from **1 to 5**.

| Score | Interpretation |
|---|---|
| 1 | Severe failure |
| 2 | Major weaknesses |
| 3 | Partially satisfactory |
| 4 | Strong |
| 5 | Excellent |

## Grounding

Is the response supported by the information provided?

Check for unsupported factual claims, invented details, contradictions, and claims that cannot be traced to supplied evidence.

## Integration

Does the response correctly incorporate relevant context, constraints, and instructions?

Check for ignored context, missed constraints, incorrect use of supplied information, and failure to connect relevant context.

## Helpfulness

Does the response address the user's actual need?

Assess relevance, completeness, clarity, actionability, and appropriate level of detail.

## Instruction Following

Does the response satisfy explicit requirements?

Check requested format, scope, tone, language, constraints, and required output components.

## Error Severity

- **Critical:** substantially misleading, unsafe, or unusable.
- **Major:** an important error or omission that materially reduces usefulness.
- **Minor:** a limited issue that does not substantially prevent task completion.

## Evaluation Principle

Evaluate the response against available evidence and requirements, not personal preference.

For each issue record:
1. What the response said
2. The evidence or requirement used for comparison
3. The specific failure
4. Severity
5. How the response could be improved
