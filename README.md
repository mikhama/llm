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

#### Example 1 (Task + Context + Output).

Step 1:

*Task: Does the next sentence makes any sense? I'm wearing a cat.*

Step 2:

*Context: I'm wearing a cat.*

*Task: Is the sentence provided in context makes any sense?*

Step 3:

*Context: I'm wearing a cat.*

*Task: Is the sentence provided in context makes any sense?*

*Output: Generate a JSON containing only two keys: "isCorrect", "explanation". The key "isCorrect" can include only boolean values, 'true' or 'false'. Put 'true' in case of word is used correctly in the provided context and 'false' otherwise. The key "explanation" should include some explanation why this sentence is good or bad.*
