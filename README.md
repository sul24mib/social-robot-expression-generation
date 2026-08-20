# Language-Conditioned Expressive Behavior Generation for Social Robots


##Background

Social robots need to communicate not only information, but also social intent.
Facial expressions help robots communicate emotions such as encouragement,
empathy, and excitement.

However, designing these behaviors manually requires researchers to specify
individual facial movements for each scenario.

Recent work has explored using large language models to generate more
context-aware robot behaviors. This project investigates whether LLMs can
generate expressive behaviors that can be directly executed by a robot face.


## Related Work

### PyLips

PyLips is an open-source platform for creating expressive robot faces.
It allows researchers to control facial behaviors through programmable
interfaces.

This project uses PyLips as the target platform for rendering generated
expressions.

Link:
https://pylips.readthedocs.io/


### LLM-Based Robot Expression Generation

Recent work has shown that language models can generate context-aware
robot behaviors by reasoning about conversational situations.

This project builds on this idea by exploring an LLM-to-expression pipeline.

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
* 

## Future Research Direction
A longer-term research goal is exploring whether expression representations can transfer across different robot embodiments.
