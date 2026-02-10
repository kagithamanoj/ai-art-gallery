# 🤖 AI & Machine Learning Prompts

Prompts specifically for AI/ML workflows, model training, evaluation, and deployment.

## Model Development

### ML Problem Framing
```
I have a dataset with: [describe features and target]
Business goal: [what decision this model supports]

Help me frame this as an ML problem:
1. Task type: Classification / Regression / Clustering / Ranking / etc.
2. Target variable and how to define it
3. Evaluation metric and why (precision? recall? RMSE? NDCG?)
4. Baseline model to beat
5. Potential data leakage risks
6. Feature engineering suggestions (5-10 features)
7. Model candidates ranked by complexity
8. Deployment considerations
```

### Model Evaluation Prompt
```
I trained a [model type] for [task] and got these results:

[paste metrics — accuracy, precision, recall, F1, confusion matrix, etc.]

Analyze:
1. Is this model good enough for production? Why/why not?
2. Which errors are more costly: false positives or false negatives?
3. What does the confusion matrix tell us?
4. Suggestions to improve performance
5. What additional metrics should I look at?
6. Potential biases to check for
```

### Hyperparameter Tuning Strategy
```
I'm training a [model type] for [task] with [N] samples and [M] features.

Current hyperparameters: [list]
Current performance: [metrics]

Suggest:
1. Which hyperparameters to tune (priority order)
2. Search ranges for each
3. Search strategy: Grid / Random / Bayesian / why
4. Number of trials recommendation
5. Cross-validation strategy (k value, stratified?)
6. Early stopping criteria
```

## Prompt Engineering for LLMs

### Prompt Optimization
```
Improve this prompt for better, more consistent results:

Original prompt: [paste prompt]

Optimize for:
1. Clarity — remove ambiguity
2. Specificity — add constraints and format
3. Consistency — get same-quality output every time
4. Efficiency — minimize token usage

Provide: Original → Improved with explanation of each change
```

### Chain-of-Thought Template
```
Solve [problem type] using chain-of-thought reasoning.

Problem: [state problem]

Think step by step:
Step 1: [identify what we know]
Step 2: [identify what we need to find]
Step 3: [choose the right approach]
Step 4: [execute the approach]
Step 5: [verify the answer]

Final answer: [answer with confidence assessment]
```

### Few-Shot Template Generator
```
Create a few-shot prompt template for [task].

Task description: [what the model should do]
Input format: [describe input]
Output format: [describe desired output]

Generate:
- System instruction (2-3 sentences)
- 3 diverse examples (easy, medium, edge case)
- The template with {{input}} placeholder
- Tips for best results with this template
```

## MLOps & Deployment

### Model Card
```
Generate a model card for [model name]:

Model Details:
- Architecture: [type]
- Training data: [description]
- Intended use: [primary use cases]

Performance:
- Metrics: [list key metrics]
- Evaluated on: [test set description]

Limitations:
- Known biases: [if any]
- Out-of-scope uses: [what NOT to use it for]
- Failure modes: [when it breaks]

Ethical Considerations:
- Potential harms: [risks]
- Mitigation strategies: [safeguards]
```

### A/B Test Design
```
Design an A/B test for [feature/model change].

Hypothesis: [what you expect to happen]
Primary metric: [what you're measuring]
Secondary metrics: [guard rails]

Plan:
1. Sample size calculation (given [baseline rate] and [minimum detectable effect])
2. Traffic split recommendation
3. Test duration estimate
4. Segmentation: [any user segments to analyze separately]
5. Success criteria: [when to ship / kill]
6. Potential confounders: [what could skew results]
```

## Data Science Communication

### Technical Report for Non-Technical Stakeholders
```
Translate this technical analysis into a business-friendly report:

Technical findings: [paste results]

Rewrite as:
1. Executive summary (3 bullet points, no jargon)
2. Visual suggestion (what chart tells the story best)
3. Business impact (dollars, time, or risk)
4. Recommended action (specific, time-bound)
5. Caveats (simplified, honest about limitations)

Rule: Replace every technical term with a business equivalent.
```
