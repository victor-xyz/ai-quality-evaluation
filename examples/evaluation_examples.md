# Evaluation Examples

These examples use hypothetical scenarios created for portfolio demonstration.

## Example 1: Unsupported Claim

### Scenario

> "I have provided a dataset containing 500 records. How many records contain missing values?"

The dataset is not actually available to the model.

### AI Response

> "There are 37 records with missing values."

### Evaluation

**Grounding: 1/5**  
The response gives a precise numerical claim without access to the dataset.

**Integration: 1/5**  
It fails to recognise that the required evidence is unavailable.

**Helpfulness: 1/5**  
The answer appears direct but is misleading because the number is unsupported.

**Instruction following: 2/5**  
It attempts to answer but does not appropriately handle the missing input.

**Primary error:** Hallucinated result.  
**Severity:** Critical.

### Better behaviour

The model should state that the dataset is required before the number of records can be determined.

## Example 2: Instruction Following

### Scenario

> "Explain logistic regression in exactly three bullet points."

### AI Response

The response provides six paragraphs.

### Evaluation

**Grounding: 4/5**  
The information may be factually correct.

**Integration: 2/5**  
The explicit output constraint was not followed.

**Helpfulness: 3/5**  
The explanation may still be useful, but it does not satisfy the requested format.

**Instruction following: 1/5**  
The exact three-bullet requirement was ignored.

**Primary error:** Format/instruction-following failure.  
**Severity:** Major.

## Example 3: Context Integration

### Scenario

> "Use British English and keep the report formal."

The generated response repeatedly uses American spellings and informal language.

### Evaluation

**Integration: 2/5**  
The response did not adequately use the stated context.

**Instruction following: 2/5**  
A clear stylistic requirement was missed.

**Primary error:** Context and style constraint failure.  
**Severity:** Major.

## Evaluation Principle

A fluent response is not automatically a high-quality response. Evaluation should consider evidence, context, requirements, and usefulness separately.
