# Lab11

## Exercise 1: Resume Screening

1. Interview rate (AI decision, score ≥ 70)

Males: 46 out of 50 = 92%  
Females: 24 out of 50 = 48% 

2. Actual qualification rate (Human Expert)
Males: 38/50 = 76%
Females: 35/50 = 70%

3. AI Accuracy by Group:

- For males: 46 got interviews and only 38 are qualified, so at best the AI caught all 38 of 38 qualified men. It passed at least 8 unqualified men.
- For females: only 24 got interviews but 35 are qualified, so at most 24 of 35 qualified women were found.
- AI Accuracy for males: 100%
- AI Accuracy for females: 68.6%

4. False negatives (qualified but rejected)

- Males: How many qualified men were scored below 70? 4.
- Females: How many qualified women were scored below 70? 11

5. Real-world Impact

- If TechCorp hires 20 people, how many would likely be male vs female based on AI recommendations?
Hiring 20 in proportion to the pool gives 20 × 46/70 ≈ 13 men and 20 × 24/70 ≈ 7 women.

- Is this proportional to the actual qualification rates?
Hiring 20 in proportion to actual qualifications (38 M vs 35 F) gives 20 × 38/73 ≈ 10 men and 10 women. So it is not proportional. The two groups are almost equally qualified (76% vs 70%), but men get nearly twice as many hires.


6. Reflection

- What evidence of bias do you see in this AI system? 
The 6-point gap in qualification turns into a 44-point gap in interview rates (92% vs 48%).
Female scores are about 10 points lower on average, and the whole female distribution sits lower.
The AI makes different kinds of errors for each group. It is too lenient with men (it passes unqualified ones) and too harsh with women (it rejects at least 11 qualified ones).

- How might this bias have developed during programming/training?  
This could have developed through training data: if the model learned from past hires in a male-dominated field, "looks like past hires" ends up meaning "looks for male."

- What would you recommend to fix this system?
Recheck outcomes by demographic group on a regular basis.
Remove names and gender, and retrain on balanced data with fair labels.
Keep a human reviewer, especially for scores near the cutoff (for example 60–70).
Be transparent with candidates and give them a way to appeal.

## Exercise 2: Transparency

1. Emotional impact: Round 1 feels frustrating, dismissive, and powerless. Round 2 is still disappointing, but it feels respectful and fair because I can see the reasoning.

2. Understanding: Round 2 is easier to understand. The most helpful information is the factor weights and the specific weak areas: the missing SAT scores (45/100) and no leadership (20/100).

3. Trust: I trust the transparent system in round 2 more, because its decisions can be checked and challenged. A black box asks for trust without giving any reason for it. 

4. Actionability: Only in Round 2 can Sarah act. She can take the SAT and add leadership roles. Raising those two scores could get her past 75. In the medical case, the patient knows to get confirmatory tests and that changes to activity level and BMI could lower the risk. Without this kind of feedback, people can't improve or contest an unfair decision.

5. Programming implications

- Explainable AI provides accountability, ability to detect bias, debugging, and earn user trust better.
- Challenges: complex models like deep learning are hard to interpret, there's a trade-off between accuracy and interpretability, explanations can reveal proprietary details or let people cheat the system.
- Ethical problem: without transparency, bias goes unnoticed, people can't appeal, and no one is held responsible for decisions that affect users.

6. Group discussion Questions:

- Should all AI systems explain their decisions? High-stakes decisions (jobs, loans, health, justice) should. Low-stakes ones like movie recommendations need less.
- Can transparency be harmful? Yes, for example by revealing fraud-detection rules, people can get around them.
- How detailed should explanations be? The level of detail should increase with the stakes and match what the audience can understand.
