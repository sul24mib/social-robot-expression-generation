# Project Scope

## Goal
Develop a system that converts conversational context into expressive robot facial behaviors.

## Motivation
Current robot expressions often require manual design. Large language models may provide a way to generate more adaptive expressive behaviors.

## Research Question
How can language models generate appropriate facial expressions for social robots?

## Deliverables
- LLM expression generation pipeline
- Expression representation
- PyLips integration
- Evaluation framework
## Work Completed
- Initial repository setup and research artifact structuring.
- System architecture definition (LLM -> JSON Expression -> PyLips -> Robot).
- Definition of baseline JSON schema for robot facial expressions (`examples/example_expression.json`).
- Literature review covering FACS, PyLips, and social robotics context.

## Remaining Work & Timeline
- **Phase 1: Pipeline Setup** – Implement basic LLM prompt engineering to output formatted JSON expressions.
- **Phase 2: PyLips Integration** – Connect JSON output to PyLips motor control interface.
- **Phase 3: Evaluation** – Conduct user studies and comparative testing.

## Evaluation Plan
- **Baseline Comparison:** Compare LLM-generated expressions against rule-based mappings and human-designed baselines.
- **Metrics:**
  - *Context Appropriateness:* Do observers feel the expression fits the text?
  - *Social Intent:* Is the intended emotion/intent accurately communicated?
  - *Latency/Execution:* Measure time taken from language input to robot movement.
