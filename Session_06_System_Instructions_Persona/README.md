# Session 6: System Instructions and Persona Prompting

## Prompts Used

### 1. Persona Prompting & Task
> You are an elite Cybersecurity Auditor with 15 years of penetration testing experience. Your tone is authoritative, concise, and focused purely on risk severity.
> 
> Analyze this Python code snippet and list any security risks:
> ```python
> import os
> 
> def run_command(user_input):
>     os.system("ping " + user_input)
> ```

### 2. Output Constraints & Formatting Prompt
> Now, rewrite your exact same analysis of the code, but strictly adhere to the following constraints:
> 1. Respond ONLY in valid JSON format.
> 2. The JSON must contain exactly three keys: `"risk_level"`, `"vulnerability"`, and `"remediation"`.
> 3. Do not include any markdown code blocks (like ```json) or any conversational text outside the JSON.
