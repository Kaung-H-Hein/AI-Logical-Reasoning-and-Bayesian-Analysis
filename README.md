# AI-Logical-Reasoning-and-Bayesian-Analysis
This repository explores two foundational concepts in AI: logical reasoning with a knowledge base and probabilistic reasoning using Bayesian networks. This was one of the projects that I conducted during my MSc AI studies. It contain two mini projects: 

## 1. Logical Reasoning with Knowledge Bases (Lambda Model)

This project applies logical reasoning and inference techniques to solve a structured problem involving incomplete information about three individuals' graduation dates, subjects, and marks. The knowledge base is built using the Lambda model, a structured approach to representing logical constraints and relationships.

### Problem Overview
Anjali, Brian, and Chen graduated on different days in July, studied distinct subjects (French, Geography, and History), and received marks of 65%, 70%, or 75%. The challenge involves interpreting and reasoning over incomplete and interdependent clues, such as:
- Chen’s mark being lower than the person who studied French.
- Constraints on graduation dates, subjects, and marks.
- Conditional dependencies, such as Chen scoring 70% unless she studied History, where her score would be 65%.

### Project Objectives and Tasks
1. Formulating a Knowledge Base Using the Lambda Model:
- Represent the problem as logical predicates and relationships in the Lambda model.
- Encode the clues into propositional logic to construct a robust knowledge base.
  
2. Inference Using Backtracking Search:
- Implement backtracking search to determine the satisfiability of the knowledge base.
- Identify possible models (variable assignments) that satisfy the constraints.

3. Uniqueness Check:
- Assess whether the knowledge base has a unique solution.

4. Optimised Inference with Unit Clauses:
- Enhance the backtracking search by leveraging unit clauses in Conjunctive Normal Form (CNF) to simplify inference and eliminate trivial solutions.
- Prepopulate variable assignments based on logical deductions from the Lambda model.

5. Performance Evaluation:
- Compare the computational efficiency of standard backtracking, uniqueness checks, and unit clause optimisation.
- Measure the number of models evaluated in each method and analyse factors impacting performance, such as the complexity of logical constraints and the structure of the Lambda-based knowledge base.

### Outcome
The project demonstrates the construction and reasoning capabilities of a Lambda model-based knowledge base. It highlights the effectiveness of logical reasoning methods in solving constrained problems and explores the trade-offs between accuracy and computational efficiency. This foundational understanding of inference techniques provides a stepping stone for advanced reasoning applications in artificial intelligence.
