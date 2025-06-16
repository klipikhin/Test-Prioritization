# Test Case Prioritization for CI with Q-Learning

**Test Case Prioritization for Continuous Integration (CI)** applies reinforcement learning to improve CI efficiency by ordering test cases to reduce feedback loops and detect failures earlier.

---

## Motivation

In modern CI environments, running the entire test suite after every change is time-consuming. Prioritizing test cases to detect bugs quickly can significantly improve feedback time and developer productivity.

---

## Approach

I designed and implemented a Q-learning agent that learns an optimal policy for ordering test cases based on historical test execution outcomes and durations.

**Key Steps:**

1. **Environment Modeling** – Represent each CI build as a sequence of test case executions with state defined by test outcomes and features.
2. **Rewards** – Assign higher rewards for early detection of failed tests and penalize long durations.
3. **Q-learning** – Train an agent over multiple epochs to learn efficient prioritization policies.
4. **Evaluation** – Compare against baseline strategies (random order, chronological) using metrics like time to first failure and average feedback time.

---

##  Usage

  **Run in Google Colab**
   - Open `test_prioritization.ipynb`
   - Execute cells from top to bottom to train and evaluate the Q-learning agent.

---
##  Project Report

A detailed explanation of the problem, algorithm design, reward engineering, and evaluation.

 [Download the full report (PDF)](qlearning.pdf)

---

##  Presentation

A quick walkthrough of the motivation, method, and results.

 [Watch the video](https://youtu.be/PNEWNb-BRL0)
