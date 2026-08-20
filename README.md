# Language-Conditioned Expressive Behavior Generation for Social Robots

## Overview

Social robots communicate using both speech and nonverbal behaviors.
However, many robot facial expressions are manually designed, making it
difficult for robots to generate context-aware expressions dynamically.

This project explores using large language models (LLMs) to generate
expressive robot behaviors from conversational context.

## Research Question

Can a language model generate context-appropriate facial expressions
for a social robot?

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
‘''
## Example

Input:

"The user successfully completed a difficult rehabilitation exercise."

Robot response:

"Great job! You did it!"

Generated expression:

```json
{
 "intent": "encouragement",
 "smile": 0.8,
 "eyebrow_raise": 0.3,
 "duration": 2.0
}
