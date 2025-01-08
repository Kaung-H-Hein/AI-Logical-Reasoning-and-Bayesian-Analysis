# AI-Logical-Reasoning-and-Bayesian-Analysis
This repository contains two mini-projects that explore key concepts in artificial intelligence: logical reasoning with knowledge bases and probabilistic reasoning using Bayesian networks. These projects were conducted during my MSc in Artificial Intelligence. The first project focuses on logical reasoning, where a knowledge base is built and used for inference tasks. The second project delves into the design and evaluation of Bayesian networks, applied to weather-related human behaviour prediction. Both projects showcase AI methods for problem-solving and inference, providing a foundational understanding of reasoning techniques in AI.

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

## 2. Bayesian Networks and Probabilistic Inference

In this mini-project, the aim is to design and evaluate Bayesian networks to model the relationships between weather conditions and human behaviour. The dataset provided includes joint probability distributions for five variables: season, temperature, rain, wearing a coat, and carrying an umbrella.

### Problem Overview
This project explores how various weather conditions influence decisions such as wearing a coat or carrying an umbrella. The key variables in the model include:
- Season (Spring, Summer, Autumn, Winter)
- Temperature (Cold, Mild, Hot)
- Rain (Raining, Not Raining)
- Wearing a Coat (Coat, No Coat)
- Carrying an Umbrella (Umbrella, No Umbrella)

### Project Objectives and Tasks
1. Design Bayesian Networks:
- Propose three different Bayesian network structures to model the relationships between the variables.
- Factorise the joint probability distribution into conditional distributions based on the chosen network structure.
- Evaluate each network for its ability to explain the joint probability distribution and how the factorisation aligns with the observed data.

2. Perform Inference:
- Conduct six inference tasks, such as calculating conditional probabilities (e.g., 𝑃(Temperature∣Umbrella), probability of the temperature given that an umbrella is being carried), and compare the results across the different network structures.

3. Evaluate Network Designs using Inference Models:
- Assess the performance of each network in terms of accuracy, computational efficiency, and how well it captures the underlying causal relationships.
- Three different inference models were used to evaluate the Bayesian networks:
  i. Exact Inference: This method calculates precise probabilities directly from the network. While accurate, it is computationally expensive and best suited for models with relatively few variables and simple structures.
  ii. Direct Sampling: This approach generates random samples from the Bayesian network to estimate probabilities. It is computationally more efficient than exact inference, though the results are approximate, with a margin of error of ±0.01.
  iii. Markov Chain Monte Carlo (MCMC): MCMC generates samples through a random walk, where each sample depends on the previous one. It's a powerful method, especially for complex networks, but also computationally intensive. Conditional independence can be enforced using functions like pm.Deterministic, although this becomes complex with high-dimensional arrays.

### Outcome
This project demonstrates the application of Bayesian networks in modelling complex probabilistic relationships, including the factorisation of the joint distribution into conditional probabilities. It highlights how different design choices, such as network structure and inference method, influence the results.

The project also shows the trade-offs between accuracy and computational efficiency. While exact inference is accurate, it is limited in scalability for more complex models. Sampling methods like Direct Sampling and MCMC are more efficient, but they come with slight approximations. Ultimately, the results from these methods offer valuable insights into selecting the most effective model and inference approach for real-world applications in probabilistic reasoning.
