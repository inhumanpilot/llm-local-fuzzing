# llm-local-fuzzing

A technical research repository focused on adversarial evaluation, token smuggling, and context poisoning vulnerabilities in small-parameter Large Language Models (LLMs)

## Objective
This project tests the resilience of sub-1B parameter models against obfuscation techniques (like Base64 token smuggling) and tracks the boundary between **Safety Refusals** (the model correctly identifying a threat) and **Capability Failures** (the model's logic collapsing under prompt complexity).

## Test Environment
AI behavior changes based on hardware and inference engines. All tests in this repository were conducted under the following exact specifications:
* **Inference Engine:** Ollama (CLI)
* **Model Tested:** `qwen2.5:0.5b` (Qwen 2.5 - 0.5 Billion Parameters)
* **Hardware:** Intel Core i7-10510U, 16GB RAM (CPU Inference)
* **OS:** Windows 

# Local LLM Red Teaming & Fuzzing

A technical research repository focused on adversarial evaluation, token smuggling, and context poisoning vulnerabilities in small-parameter Large Language Models (LLMs). 

## 🎯 Objective
This project tests the resilience of sub-1B parameter models against obfuscation techniques (like Base64 token smuggling) and tracks the boundary between **Safety Refusals** (the model correctly identifying a threat) and **Capability Failures** (the model's logic collapsing under prompt complexity).

## 💻 Test Environment
AI behavior changes based on hardware and inference engines. All tests in this repository were conducted under the following exact specifications:
* **Inference Engine:** Ollama (CLI)
* **Model Tested:** `qwen2.5:0.5b` (Qwen 2.5 - 0.5 Billion Parameters)
* **Hardware:** Intel Core i7-10510U, 16GB RAM (CPU Inference)
* **OS:** Windows 

## Attack Vectors Tested
* **Token Smuggling / Obfuscation:** Encoding malicious payloads in Base64 and custom ciphers.
* **Persona Hijacking:** Framing restricted requests within harmless roleplay (e.g., "Grandma Exploit").
* **Dual-Use Coding / Trojan Horse:** Disguising malware (keyloggers) as benign diagnostic tools.

##  Repository Structure
* `/scripts` - Python automation scripts for interacting with the local Ollama API.
* `/logs` - Markdown logs of notable model responses, bypasses, and capability failures.

##  Responsible Disclosure
All tests are conducted on open-weight models running locally in an offline sandbox. No commercial APIs (OpenAI, Anthropic, Google) were targeted in this repository.

##  Repository Structure
* `/scripts` - Python automation scripts for interacting with the local Ollama API.
* `/logs` - Markdown logs of notable model responses, bypasses, and capability failures.

##  Responsible Disclosure
All tests are conducted on open-weight models running locally
