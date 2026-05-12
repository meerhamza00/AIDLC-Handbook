# Module 1: Ideation & Requirement Synthesis
## Transforming the "What" (Product Discovery)

In the traditional PDLC, ideation is often a bottleneck of endless meetings, vague emails, and manually written PRDs (Product Requirement Documents) that are outdated the moment they are saved.

### 1. The Contrast: Traditional vs. AI-Powered

| Activity | Traditional Method | AI-Powered Method (AIDLC) |
| :--- | :--- | :--- |
| **Market Research** | Manual browsing, reading reports, interviews. | AI-driven synthesis of competitor reviews, social sentiment, and trend analysis. |
| **User Personas** | "Imaginary" profiles based on generic assumptions. | **Synthetic Personas:** LLM-simulated users built from real data to "interview" and stress-test features. |
| **Requirement Drafting** | Manual writing of User Stories and Acceptance Criteria. | **Rapid Prototyping of PRDs:** AI generates the first draft; human curates and refines the constraints. |
| **Edge-Case Analysis** | Relying on the lead dev's experience to "spot" errors. | **Adversarial Prompting:** Asking AI to "act as a malicious user/edge-case generator" to find gaps in logic. |

### 2. The AI-Powered Workflow: Step-by-Step

#### Step A: Concept Expansion
Instead of a brainstorming meeting, use a "Recursive Expansion" prompt.
**The Loop:** Concept $\rightarrow$ AI expands into 5 directions $\rightarrow$ Human selects 1 $\rightarrow$ AI breaks that direction into 10 specific features.

#### Step B: Synthetic User Testing
Before writing a single line of code, create a "Synthetic Panel."
1. Define 3 distinct personas (e.g., "The Power User," "The Non-Tech Novice," "The Security Skeptic").
2. Feed the product concept to the AI and ask: *"Based on these personas, what are the top 3 reasons they would HATE this product?"*
3. Pivot the requirements based on this simulated friction.

#### Step C: The "Executable" PRD
Stop writing PRDs as static documents. Write them as **Instruction Sets for Agents**.
A modern PRD should include:
- **The Core Objective:** A clear, unambiguous goal.
- **Constraints:** Technical, legal, and design boundaries.
- **Success Metrics:** How the AI can verify the feature is "done."

### 🧪 The Lab: Requirement Synthesis
**Exercise: The "Anti-PRD"**
1. Write a simple 1-paragraph idea for a feature.
2. Use this prompt: *"I have an idea for [FEATURE]. Act as a world-class Product Manager. Tell me why this is a bad idea, what similar products failed at, and 5 critical edge cases I have completely ignored."*
3. Use the output to refine your requirements.

**Conclusion:** In AIDLC, the goal of ideation isn't to "get it right" on the first page, but to **rapidly simulate failure** so that the eventual build is bulletproof.
