# Deep Dive into Gemini CLI

Memory or context is provided via the `GEMINI.md` file to supply information or store conversation history. The `GEMINI.md` file can be initialized and located at different levels within your project directory structure.

## 1. Root/Home Directory

This level is mainly used to define rules and governing principles that should be applied to **every** project.

### When To Use
It can be used for the following use cases:
*   Initialize comments before each feature in every project.
*   Instruct the LLM to respond in a specific language (e.g., Roman Urdu).
*   Declare tests before each functionality of each project (TDD).

### Real World Resemblance
*   **Principle:** Behave gently, talk politely, and meet with good etiquette & ethics with everyone, everywhere.
*   **Analogy:** These are your root-level principles that you acquire and carry everywhere, influencing everyone intentionally or unconditionally.

## 2. Project Root Directory

This level is used to set instructions for a **specific project directory** without influencing any other project.

### When to Use
*   To define the project's tech stack (e.g., Frontend: Next.js, Backend: Python & FastAPI, Database: MongoDB or MySQL).

### Real World Resemblance
*   **Context:** Consider your home as a **Project Level**, Workspace as your **Root Level**, and Yourself as a **Module/Component**.
*   **Scenario:** If you are at home (Project Directory) and get tired, you take a rest or nap.
*   **Constraint:** This is a Project Root Level rule. It shouldn't influence your manners/ethics (Root Level). For example, if you are outside the home (at a workspace) and get tired, you typically can't just take a nap there.
*   **Impact:**
    *   **Routine (Module Level):** If exams are coming up, you focus on studies, restricting leisure activities. This impacts your routine (Modular Level) but doesn't change your home rules (Project Level) or your core ethics (Root Level).

### Key Takeaway
*   **Root Level (`.gemini/GEMINI.md`):** Influences every project and module.
*   **Project Level (`project/GEMINI.md`):** Influences only that specific project, not others.
*   **Module Level (`project/module/GEMINI.md`):** Influences only that specific module/component.

## 3. Sub Folder/Module/Component Level

This is used to set instructions or provide specs/details for a **specific feature** within a specific project directory.

### Real World Scenarios
*   **Context:** Consider yourself as the Component/Module.
*   **Scenario:** Your personal plans (e.g., "On weekends, I will take a rest or spend time with family").
*   **Impact:** This only impacts you or your routine work. This is your Module/Component Level.

---

## FAST API Setup

### 0. Initialize Project
Initialize a project through the `uv` package manager (10-100x faster than pip).

### 1. Virtual Environment
Create and activate a virtual environment to maintain project dependencies.

### 2. Prompt Work
Make an instance and endpoints.

### Start the Server
```bash
uv run uvicorn main:app --reload
```
