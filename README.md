# Language-Conditioned Expressive Behavior Generation for Social Robots

## Overview

Social robots communicate using both speech and nonverbal behaviors. However, many robot facial expressions are manually designed, making it difficult for robots to generate context-aware expressions dynamically.

This project explores using large language models (LLMs) to generate expressive robot behaviors from conversational context.

## Research Question

Can a language model generate context-appropriate facial expressions for a social robot?

## Proposed System

```text
Conversation Context
        │
        ▼
       LLM
        │
        ▼
Expression Representation
        │
        ▼
      PyLips
        │
        ▼
Robot Facial Expression
```

## Example

**Input:**
> "The user successfully completed a difficult rehabilitation exercise."

**Robot response:**
> "Great job! You did it!"

**Generated expression:**
```json
{
 "intent": "encouragement",
 "smile": 0.8,
 "eyebrow_raise": 0.3,
 "duration": 2.0
}
```

## Project Goals
* Develop a pipeline from language to robot facial expressions.
* Create an interpretable expression representation.
* Evaluate whether generated expressions match conversational context.

## Evaluation Plan
**Compare:**
* Rule-based expression generation
* LLM-generated expression generation

**Evaluate:**
* Context appropriateness
* Communication of social intent
* Expression quality

## Future Research Direction
A longer-term research goal is exploring whether expression representations can transfer across different robot embodiments.
