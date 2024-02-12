# LLM Workshop

## Prompt Engineering

### Prompt Components
- Role
- Context
- Task
- Data
- Output
- Example
- Constraints
- Evaluation Criteria

#### Example 1 (Task + Context + Output)

**Step 1**

Does the next sentence makes any sense? I'm wearing a cat.

**Step 2**

Context: I'm wearing a cat.

Task: Is the sentence provided in the context makes any sense?

**Step 3**

Context: I'm wearing a cat.

Task: Is the sentence provided in the context makes any sense?

Output: Generate a JSON containing only two keys: "isCorrect", "explanation". The key "isCorrect" can include only boolean values, 'true' or 'false'. Put 'true' in case of word is used correctly in the provided context and 'false' otherwise. The key "explanation" should include some explanation why this sentence is good or bad.

#### Example 2 (Task + Role)

**Step 1**

What do you prefer fish or chicken?

**Step 2**

Role: Act as a cat.

Task: What do you prefer fish or chicken?

#### Example 3 (Task + Data + Context + Constraints)

**Step 1**

Task: Propose which candidate is better for a position of Software Engineer.

Data: \
Name,Education,Experience in IT,Expected salary (USD),Skills
Olivia Johnson,Software Engineer,10 years,5000,React;Node.js;AWS;TypeScript
Liam Smith,Lawyer,2 years,4000,React;Angular;TypeScript
Sophia Williams,Teacher,student - no experience,2000,JavaScript;Chat GPT;React
Noah Brown,Dentist,3 years,5500,JavaScript;AWS;Gen AI;ML

**Step 2**

Context: Our company has recently got an opportunity to participate in a new state-of-the-art application which is aimed to help people to recognize problem with their teeth on early stages. Developing of this product involes not only classical technologies used for developing web applications, but knowledge in the field of dentistry and medicine as well as knowledge in AI.

Task: Propose which candidate is better for a position of Software Engineer.

Data: \
Name,Education,Experience in IT,Expected salary (USD),Skills \
Olivia Johnson,Software Engineer,10 years,5000,React;Node.js;AWS;TypeScript \
Liam Smith,Lawyer,2 years,4000,React;Angular;TypeScript \
Sophia Williams,Teacher,student - no experience,2000,JavaScript;Chat GPT;React \
Noah Brown,Dentist,3 years,5500,JavaScript;AWS;Gen AI;ML

**Step 3**

Context: Our company has recently got an opportunity to participate in a new state-of-the-art application which is aimed to help people to recognize problem with their teeth on early stages. Developing of this product involes not only classical technologies used for developing web applications, but knowledge in the field of dentistry and medicine as well as knowledge in AI.

Task: Propose which candidate is better for a position of Software Engineer.

Data: \
Name,Education,Experience in IT,Expected salary (USD),Skills \
Olivia Johnson,Software Engineer,10 years,5000,React;Node.js;AWS;TypeScript \
Liam Smith,Lawyer,2 years,4000,React;Angular;TypeScript \
Sophia Williams,Teacher,student - no experience,2000,JavaScript;Chat GPT;React \
Noah Brown,Dentist,3 years,5500,JavaScript;AWS;Gen AI;ML

Constraints: \
Consider only candidates which expected salary is below $5000.

#### Example 4 (Task + Example)

**Step 1**

Write a list of sentences with mistakes.

**Step 2**

Task: Write a list of sentences with mistakes.

Example: I'm eating apple. -> I'm eating an apple.
You is my boss. -> You are my boss.

#### Example 5 (Task + Evaluation Criteria)

**Step 1**

