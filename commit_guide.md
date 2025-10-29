## **📜 Commit Message Guidelines (Clean & Flexible)**

### **1. Structure**

```
<type>: <short summary>

[Optional body]

[Optional footer]

```

- **`<type>`** — a keyword that indicates the nature of the change.
- **`<short summary>`** — one concise sentence in **present tense** (max ~50 chars).
- **Body** (optional) — explain **why** and/or **how**, wrapped at ~72 chars.
- **Footer** (optional) — references like issue numbers, breaking changes.

### **2. Allowed `<type>` Values**

Keep it minimal but descriptive:

- **feat** — new feature
- **fix** — bug fix
- **refactor** — restructuring without changing behavior
- **perf** — performance improvements
- **docs** — documentation changes
- **style** — code style changes (formatting, linting; no logic change)
- **test** — adding or modifying tests
- **chore** — maintenance tasks (build scripts, dependencies, config)

---

### **3. Writing Rules**

- Use **present tense**: `"Add"`, not `"Added"` or `"Adds"`.
- Keep **summary short**: ~50 characters or less.
- First letter of summary **lowercase** unless it's a proper noun.
- No ending period in summary.
- If body is needed, leave **one blank line** between summary and body.
- Explain *why* the change was made, not just *what*.
- Multiple changes? **Split into multiple commits**.

---

### **4. Examples**

### Good:

```
feat: add search filter to task list
ex) feat: add keyword and category filters to improve task search usability

fix: prevent crash on empty user profile
ex) fix: handle null user data on startup to prevent app crash

refactor: simplify API response parsing logic
ex) refactor: merge redundant parsing functions into unified response handler

docs: update setup instructions for Windows
ex) docs: clarify venv activation and dependency install steps for Windows users

test: add unit tests for login service
ex) test: cover login success and invalid credentials cases in LoginService tests

perf: reduce image load time by caching
ex) perf: implement local image cache to reduce loading time and API calls

chore: upgrade dependencies and clean scripts
ex) chore: bump project dependencies and remove unused build scripts
```

### With body:

```
fix: handle null values in category field

This prevents the app from throwing an exception when
loading old tasks without a category in the database.

```

---

### **5. Flexibility Notes**

- You can **skip type** if the project is solo and context is obvious:
    
    ```
    add export button for completed tasks
    
    ```
    
- For bigger changes, link issues in footer:
    
    ```
    feat: implement calendar view for task history
    
    Closes #42
    
    ```
    
- You can combine types in rare cases, but **avoid type soup**:
    
    ```
    feat/refactor: redesign task edit flow
    
    ```
    

---

This way it’s:

- **Minimal** → easy to remember.
- **Consistent** → readable history.
- **Flexible** → no forced emoji, no over-restrictive format.
- **Scalable** → works for small or big teams.

---
