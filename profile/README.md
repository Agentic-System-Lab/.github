# Agentic System Lab

We build tools that make agentic systems easier to see, build and measure.

An agent is a model in a loop: step after step, the model proposes an action and the harness carries it out, until it stops. A chat box shows only the question and the answer. Our projects open up the loop in between, with models that run on your own machine, so you can watch each step instead of taking it on trust.

We're based in Taiwan. Our docs come in English and Traditional Chinese.

## Projects

### <img src="https://raw.githubusercontent.com/Agentic-System-Lab/agent-loop-visualizer/main/app/assets/logo.svg" alt="" width="24"> [Agent Loop Visualizer](https://github.com/Agentic-System-Lab/agent-loop-visualizer)

Watch an agent loop run step by step, down to every token the model writes: the token's probability, the candidates it beat, the special tokens, and the tool calls the harness reads out of them. Gemma 4 E2B or Qwen3.5 0.8B runs on your machine with `transformers`, or on vLLM. You can also try MTP speculative decoding, attach images, audio or video, give the model a Python sandbox, or hand the loop to [pi](https://pi.dev).

[![Agent Loop Visualizer: the chat on the left, the loop diagram and the tokens of one step on the right](https://raw.githubusercontent.com/Agentic-System-Lab/agent-loop-visualizer/main/docs/screenshot-en.png)](https://github.com/Agentic-System-Lab/agent-loop-visualizer)

- [How it works](https://agentic-system-lab.github.io/agent-loop-visualizer/en/): the 18 stages of one turn, each linked to the lines of code that do it
- [Experiments to try](https://github.com/Agentic-System-Lab/agent-loop-visualizer#experiments-to-try): sampling, stop conditions, human approval, MTP, images as tokens, code in a sandbox
- English | [繁體中文](https://github.com/Agentic-System-Lab/agent-loop-visualizer/blob/main/README.zh-TW.md) · Apache-2.0

More tools are on the way: one for prototyping a new agent system from an idea, and one for testing a change to an existing system against your own tasks and hardware. They'll be listed here once they're public.

## Learning together

### [Agent Atlas study group](https://agentic-system-lab.github.io/agent-atlas-learning/)

Agent Atlas strings seven courses from CMU, Stanford and Harvard into one learning path for AI agents, in 12 units. It starts with building an agent and checking what it can do, and goes on to shipping software and improving it over time. The study group follows this path, meets online and keeps shared notes. Sessions are in Traditional Chinese. Agent Loop Visualizer is the hands-on companion to Unit 01.

## How we work

- **Show the mechanism.** Each project draws what actually runs, and its docs link every step to the file and line of code that does it.
- **Run it on your own machine.** Local models let you see every token's probability, and your data stays with you.
- **Try it, don't just read about it.** Each project comes with experiments you can run to check an idea for yourself.
