# Module 1: Ideation & Requirement Synthesis
## Transforming the "What" (From Static Docs to Executable Blueprints)

In the traditional PDLC, ideation is a bottleneck of vague emails and static PRDs. In AIDLC, we treat requirements as **Input Data for Agents**.

### 1. The Contrast: Traditional vs. AI-Powered

| Activity | Traditional Method | AI-Powered Method (AIDLC) |
| :--- | :--- | :--- |
| **Market Research** | Manual browsing, reading reports. | AI-driven synthesis of competitor reviews and social sentiment. |
| **User Personas** | Imaginary profiles. | **Synthetic Personas:** LLM-simulated users based on real data to "interview" and stress-test. |
| **Requirement Drafting** | Manual writing of User Stories. | **Rapid Prototyping:** AI generates drafts; human curates constraints. |
| **Edge-Case Analysis** | Relying on seniority. | **Adversarial Prompting:** AI acts as a "malicious user" to find logic gaps. |

### 🛠 Implementation: The Advanced a-la-carte Workflow

To implement this at a professional level, don't just "ask for a PRD." Use the **Recursive Expansion** method:

#### Step A: The-Concept-Squeeze (Sourcing)
Feed the AI a broad idea and a "Sourcing Agent" prompt:
> *"Analyze the current market for [IDEA]. Find 3 successful competitors and 3 failed attempts. Synthesize the 'Common Success Pattern' and the 'Fatal Error Pattern'. Provide a set of non-negotiable requirements to avoid the fatal errors."*

#### Step B: The Synthetic Panel (Simulated Feedback)
Create 3 distinct agent personas:
1. **The Power User:** Demands efficiency and advanced shortcuts.
2. **The Non-Tech Novice:** Demands extreme simplicity and guidance.
3. **The Security Skeptic:** Demands transparency and data privacy.
**The Loop:** Present the feature to all three $\rightarrow$ Ask them to debate the feature $\rightarrow$ Resolve the conflict as the Human Architect.

#### Step C: The "Agentic" PRD (The Executable Blueprint)
A modern PRD is not a document; it is a **Configuration File** for the Coder Agent. Every requirement must include:
- **ID:** (e.g., REQ-01)
- **The Objective:** Clear goal.
- **Constraint:** "Must not use external library X," "Must run in <200ms."
- **Verification Prompt:** "How would a QA agent prove this is done?"

### ⚠️ Pitfalls & Mitigations
- **The "Yes-Man" Effect:** AI tends to tell you your idea is great. 
- **Mitigation:** Use **Adversarial Prompting**. Force the AI to act as a "Hater" or a "Competitor" to identify weaknesses.

### 🧪 The Lab: Requirement Synthesis
**Exercise: The Adversarial Persona**
1. Write a 1-paragraph feature idea.
2. Prompt: *"Act as a world-class Product Manager who hates this idea. Tell me exactly why it will fail, who will find it confusing, and 5 edge cases that will crash the system if not handled. Be brutal."*
3. Refine your PRD based on the "failures."

**Conclusion:** The goal of ideation in AIDLC is to **simulate failure as early as possible**, moving the risk from production back to the prompt.
