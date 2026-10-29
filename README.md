# local-ai-firmware-assistant.
# Local AI Firmware Assistant
*An offline, locally-hosted LLM environment for bare-metal C/C++ generation.*

## Overview
This is an internal workflow tool I configured to accelerate my embedded systems development (STM32/ESP32) without relying on cloud APIs. 

## Stack
* **Engine:** Ollama
* **Model:** Qwen 2.5 (3B parameters)
* **Environment:** Windows / WSL Ubuntu
* **Target Output:** Bare-metal C/C++

## Why Local?
1. **Zero Latency & Offline:** Allows me to work in hardware labs without internet access.
2. **Context Control:** Prevents cloud models from hallucinating hardware-specific registers by keeping the context window strictly constrained to the MCU datasheets I feed it.
3. **AI Delegation Practice:** Forcing a smaller 3B model to generate accurate C code requires breaking problems down into highly specific prompts, which improves my ability to strictly "drive" AI agents rather than blindly relying on them.
