# Retriev 

## 1. The Vision: Why Retriev?

In the age of AI, students have infinite information but face a crisis of learning. LLMs like ChatGPT are seductive shortcuts, often used for rote summarization or generating answers without fostering genuine understanding. This creates an "AI crutch," hampering critical thinking and long-term knowledge retention.

Simultaneously, decades of cognitive science have given us a clear blueprint for effective learning: Spaced Repetition, Active Retrieval, Interleaving, and more. Yet, these methods are often cumbersome to apply manually and feel disconnected from a student's actual study materials.

**Retriev is the bridge.** It is an AI-native platform that doesn't just give you answers; it actively embeds proven learning science into your study workflow. It transforms your passive course materials into an interactive, intelligent learning experience that teaches you how to learn effectively.

---

## 2. Core Features: The Student's Toolkit

Retriev is built around six core pillars, each designed to tackle a specific aspect of deep learning.

### 🧠 1. Smart Study Planner  
**Principle:** Spaced Repetition & Interleaving  
**Function:** Users input their subjects and topics for an upcoming exam. The app's algorithm automatically generates an optimized, dynamic study schedule. It intelligently interleaves topics (e.g., a bit of calculus, then some physics, then back to a different calculus concept) and schedules review sessions at scientifically-backed intervals to fight the "forgetting curve."

### ❓ 2. Retrieval & Elaboration Prompter  
**Principle:** Active Retrieval & Elaboration  
**Function:** After ingesting your study materials (lecture notes, PDFs), the platform auto-generates high-quality quizzes. It goes beyond simple flashcards by asking "why" and "how" questions. After a study session, it prompts you to explain key ideas aloud (using voice-to-text) or type a summary, forcing you to articulate and solidify your knowledge.

### 💡 3. Concrete Examples Generator  
**Principle:** Concrete Examples  
**Function:** Struggling with an abstract concept like "entropy" or "asymptotic complexity"? The LLM-powered generator provides multiple, diverse, and relatable examples and analogies to ground the idea in reality, making it intuitive and memorable.

### 🎨 4. Dual Coding Helper  
**Principle:** Dual Coding (Combining Words & Visuals)  
**Function:** The platform analyzes your text-based materials and suggests appropriate visuals. It can auto-generate simple diagrams, flowcharts, or mind maps using integrated tools like Mermaid.js, or provide a canvas with suggestions for you to sketch in an Excalidraw-like interface.

### 🤖 5. AI Usage Coach  
**Principle:** Metacognition (Thinking about thinking)  
**Function:** This is our answer to the "AI crutch." Before you can ask the integrated AI a question, it prompts you:  
“What is your goal? (A) Deeply understand a concept, (B) Memorize a fact, or (C) Analyze a problem?” Based on your answer, it guides you to ask better questions. Instead of letting you ask "Summarize this chapter," it suggests, "Ask the AI to act as a debate opponent and challenge the main arguments in this chapter."

### 📓 6. Study Reflection Journal  
**Principle:** Retrieval-Enhancing Feedback  
**Function:** At the end of each study session, you log what you learned, your confidence level, and any points of confusion. The platform provides immediate feedback, and its journaling system uses your own words to create future retrieval prompts. GPT-4 analyzes your reflections to suggest what to review next and which learning strategy to employ.

---

## 3. How It Works: The Technical Architecture

| Component    | Technology / Stack                                  | Purpose                                                                                      |
|--------------|---------------------------------------------------|----------------------------------------------------------------------------------------------|
| Frontend     | React (Next.js), TypeScript, TailwindCSS, Zustand/Redux | A highly interactive, responsive, and fast user interface for the web application.          |
| Backend API  | Node.js, Express.js, TypeScript, PostgreSQL       | Handles user authentication, data management (study sets, schedules), and core business logic. |
| AI Service   | Python, FastAPI, LangChain/LlamaIndex, PyTorch    | All heavy AI lifting. Manages document ingestion, vectorization, RAG pipelines, and LLM interactions. |
| Databases    | PostgreSQL (relational), ChromaDB / Pinecone (vector embeddings) | Securely stores user data and enables efficient similarity searches for the AI service.     |
| DevOps & Cloud | Docker, GitHub Actions, AWS / GCP (S3, EC2, RDS) | Ensures robust, automated CI/CD pipelines for testing and deployment, and scalable cloud infrastructure. |

---

## 4. Project Roadmap: From MVP to V1.0

This project follows a phased development plan to ensure consistent progress and a stable, feature-rich final product.

### Phase 1: The Core Engine (Q3-Q4 2025)
- Develop the Python AI Service for document ingestion (text/PDF).
- Implement the Retrieval & Elaboration Prompter to auto-generate quizzes.
- Build the core React frontend to display study materials and quizzes.
- Set up basic user authentication and database schemas.  
**Goal:** A user can upload a document and get a functional quiz.

### Phase 2: The Smart Scheduler (Q1 2026)
- Implement the Smart Study Planner algorithm for spaced repetition and interleaving.
- Build the user dashboard to display the daily "Cognitive Workout."
- Develop the Study Reflection Journal feature.  
**Goal:** A user has a fully functional, adaptive learning schedule.

### Phase 3: The AI Coach & Enhancers (Q2 2026)
- Build the AI Usage Coach with guided prompting logic.
- Implement the Concrete Examples Generator and Dual Coding Helper.
- Begin beta testing with a small group of students.  
**Goal:** The platform is feature-complete for an initial public release.

### Phase 4: Expansion & V1.0 (Beyond Q2 2026)
- Integration with third-party platforms (Notion, Anki, Canvas).
- Develop a native mobile app (React Native).
- Explore monetization models and institutional licensing.

---

## 5. North Star Metric: Measuring Success

While vanity metrics like user sign-ups are useful, our primary measure of success is learning effectiveness.

- **Primary Metric:** Weekly Active Learners (WALs)  
  The number of unique users who complete at least one full "Cognitive Workout" (review + reflection) cycle per week. This measures sustained engagement.

- **Secondary (Aspirational) Metric:** Verified Knowledge Retention Score (VRS)  
  A custom score calculated from a user's performance on spaced repetition quizzes over time, indicating a tangible increase in long-term memory.

---

## 6. Getting Started (Local Development)

### Clone the repository:

```bash
git clone https://github.com/your-username/cognitive-catalyst.git
cd cognitive-catalyst
