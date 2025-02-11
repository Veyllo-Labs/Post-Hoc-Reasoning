# Post-Hoc-Reasoning
A system prompt approach enabling Large Language Models (LLMs) to perform post-response reasoning without additional training.

## Overview

Post-Hoc-Reasoning introduces a novel system prompt that "teaches" LLMs to think by separating their internal reasoning process from their final answer. By incorporating `<think>` and `<answer>` tags—similar to the deepseek-r1 method—this approach allows the model to articulate its thought process before delivering the final response.

## Key Features

- **Post-Response Reasoning:** Empowers LLMs to perform a reasoning process after generating an initial answer.
- **Thought/Answer Separation:** Uses `<think>` and `<answer>` tags to clearly distinguish the reasoning phase from the final answer.
- **Wide Applicability:** Can be integrated with almost any LLM by simply applying the system prompt.
- **Tested Implementation:** Demonstrated successful results with the Gemma2:27B model in the Msty app.


## Msty Integration

For optimal performance with Msty, please follow these steps:

1. **Insert the System Prompt:**  
   Copy the content of `Reasoning prompt.md` and paste it into the **Model Options > Model Instructions** section in Msty.

2. **Configure Output Settings:**  
   - Set the **Maximum Output Tokens** to a minimum of **8000** tokens.  
   - Ensure that the **Context Window Size** is set to at least **8048** tokens.

These settings are crucial to provide the model with sufficient capacity to process the reasoning instructions effectively and generate comprehensive outputs.
