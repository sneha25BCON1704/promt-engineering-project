# Session 5: Meta-Prompting (Prompt Generation & Refinement)

## Prompts Used

### 1. Meta-Prompt (Generation)
> I want to generate a detailed, structured prompt for an AI that will act as an expert Python code reviewer. Create a complete, high-quality prompt that forces the AI reviewer to check for code efficiency, security vulnerabilities, and PEP 8 style compliance.

### 2. Code Tested with Generated Prompt
```python
def get_user_data(user_id):
    import sqlite3
    conn = sqlite3.connect('database.db')
    cursor = conn.cursor()
    query = "SELECT * FROM users WHERE id = '" + str(user_id) + "'"
    cursor.execute(query)
    return cursor.fetchall()
