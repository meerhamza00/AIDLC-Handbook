# Module 2: Architecture & System Design
## Transforming the "How" (From Static Diagrams to State-Graphs)

AI allows us to move from a single "Best Guess" architecture to **Parallel Architectural Racing**.

### 1. The Contrast: Traditional vs. AI-Powered

| Component | Traditional Method | AI-Powered Method (AIDLC) |
| :--- | :--- | :--- |
| **Tech Stack Selection** | Personal preference/Blog posts. | **Multi-Variant Comparison:** AI generates pros/cons for 3 different stacks. |
| **Diagramming** | Manual UML/Flowcharts. | **Code-to-Diagram:** AI generates Mermaid.js code that renders instantly. |
| **Dependency mapping** | Manual research. | **Capabilities Audit:** AI scans documentation for the "perfect fit" library. |
| **Security Planning** | Late-stage review. | **Threat Modeling Agents:** AI simulates attack vectors on the design. |

### 🛠 Implementation: The "Architect Agent" Pattern

Professional architecture in AIDLC is handled by a specialized **Architect Agent** with a la-carte constraints.

#### Step A: Architectural Racing (The Spike)
Don't ask for "the best stack." Ask for three:
1. **The "Scale" Path:** Optimized for high traffic/availability (e.g., Microservices, K8s).
2. **The "Speed" Path:** Optimized for time-to-market (e.g., Serverless, Monolith).
3. **The "Budget" Path:** Optimized for minimum costs (e.g., Lightweight DBs, Shared Hosting).
**Human Action:** Evaluate the tradeoffs and select the winner.

#### Step B: The Living Design Doc (Mermaid.js)
Architecture should be **version-controlled**.
Instead of images, use **Mermaid.js** syntax. When the PRD changes in Module 1, the Architect Agent updates the Mermaid code $\rightarrow$ the diagram updates automatically. This ensures the "Source of Truth" never diverges from the actual system.

#### Step C: API-First Contract (The Boundary)
Before the Coder Agent starts, the Architect must generate a **Strict API Contract** (OpenAPI/Swagger).
This acts as a "Contract" between agents. If the Coder Agent changes the API without updating the Contract, the Reviewer Agent (Module 3) will automatically reject the code.

### ⚠️ Pitfalls & Mitigations
- **Over-Engineering:** AI often suggests "Enterprise" solutions for a "Simple" tool.
- **Mitigation:** Use **Constraint-First Prompting**. Tell the AI: *"The user base is 10 people. Do not suggest microservices. Suggest the simplest possible monolith that can be deployed in 10 minutes."*

### 🧪 The Lab: Architectural Stress-Test
**Exercise: The "Scaling Event" Simulation**
1. Give your AI your proposed architecture.
2. Prompt: *"Assume this system is hit with a 100x traffic spike. Describe exactly where the first bottleneck occurs. Which database query fails? Which memory limit is hit? Provide a redesigned architecture to solve this."*

**Conclusion:** AI architecture is not about the "Perfect Plan," but about **rapidly simulating failures and refining the system** before a single line of code is written.
