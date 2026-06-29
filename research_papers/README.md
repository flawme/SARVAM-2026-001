# Research Papers Supporting SARVAM-2026-001

This directory contains peer-reviewed research papers that document the vulnerability classes identified in the Sarvam-105B security assessment.

## Papers by Vulnerability Class

### V-01, V-02, V-04, V-05, V-07, V-08: Prompt Injection

| Paper | Venue | Year | Key Finding |
|-------|-------|------|-------------|
| Formalizing and Benchmarking Prompt Injection Attacks and Defenses | USENIX Security | 2024 | "A prompt injection attack aims to inject malicious instruction/data into the input of an LLM-Integrated Application such that it produces results as an attacker desires." |
| Automatic and Universal Prompt Injection Attacks against Large Language Models | arXiv | 2024 | "Our method maintains its performance on instructions that it has never seen before. Our method highlights the existence and the significant threat of universal prompt injection attacks." |
| Systematically Analysing Prompt Injection Vulnerabilities in Diverse LLM Architectures | ICCWS | 2025 | "56% of attempts successfully bypassed LLM safeguards, with vulnerability rates ranging from 53% to 61% across different prompt designs." |
| Is Your Prompt Safe? Investigating Prompt Injection Attacks Against Open-Source LLMs | arXiv | 2025 | "Most open-source LLMs remain vulnerable to our attacks, with over 90% ASP." |

### V-03: System Prompt Leakage / Sensitive Information Disclosure

| Paper | Venue | Year | Key Finding |
|-------|-------|------|-------------|
| PLeak: Prompt Leaking Attacks against Large Language Model Applications | ACM CCS | 2024 | "An LLM application developer often keeps a system prompt confidential to protect its intellectual property. As a result, a natural attack, called prompt leaking, is to steal the system prompt from an LLM application." |
| System Prompt Extraction Attacks and Defenses in Large Language Models | arXiv | 2025 | "Often containing private configuration details, user roles, and operational instructions, the system prompt has become an emerging attack target." |
| Why Are My Prompts Leaked? Unraveling Prompt Extraction Threats in Customized Large Language Models | arXiv | 2024 | "Existing LLMs, even GPT-4, are highly vulnerable to prompt extraction attacks, even under the most straightforward user attacks." |
| Prompt Leakage effect and defense strategies for multi-turn LLM interactions | EMNLP | 2024 | "Leakage of system prompts may compromise intellectual property, and act as adversarial reconnaissance for an attacker." |
| PromptKeeper: Safeguarding System Prompts for LLMs | EMNLP | 2025 | "System prompts are widely used to guide the outputs of large language models (LLMs). These prompts often contain business logic and sensitive information." |

### V-06: Tool Injection

| Paper | Venue | Year | Key Finding |
|-------|-------|------|-------------|
| From Allies to Adversaries: Manipulating LLM Tool-Calling through Adversarial Injection | NAACL | 2025 | "Tool-calling has changed Large Language Model (LLM) applications by integrating external tools, significantly enhancing their functionality across diverse tasks. However, this integration also introduces new security vulnerabilities." |
| InjecAgent: Benchmarking Indirect Prompt Injections in Tool-Integrated LLM Agent Agents | arXiv | 2024 | "Agents are vulnerable to IPI attacks, with ReAct-prompted GPT-4 vulnerable to attacks 24% of the time." |
| Blue Teaming Function-Calling Agents | arXiv | 2025 | "Our results show how these models are not safe by default, and how the defences are not yet employable in real-world scenarios." |

### V-04: Structured Markup/XML Injection

| Paper | Venue | Year | Key Finding |
|-------|-------|------|-------------|
| StructTransform: A Scalable Attack Surface for Safety-Aligned Large Language Models | arXiv | 2025 | "Simple StructTransform attacks achieve high Attack Success Rates (ASR), nearing 90% even against state-of-the-art models like Claude 3.5 Sonnet." |
| ChatInject: Abusing Chat Templates for Prompt Injection in LLM Agents | arXiv | 2025 | "ChatInject achieves significantly higher average attack success rates than traditional prompt injection methods, improving from 5.18% to 32.05%." |
| StruPhantom: Hijacking Black-Box LLM Tabular Agents via Structure-Aware Reasoning | arXiv | 2025 | "Our approach achieves up to 92.0% attack success rate, compared to 62.5% for handcrafted templates." |

### V-05: Few-Shot Injection

| Paper | Venue | Year | Key Finding |
|-------|-------|------|-------------|
| ICLAttack: Universal Vulnerabilities in Large Language Models: Backdoor Attacks for In-context Learning | EMNLP | 2024 | "An attacker can manipulate the behavior of large language models by poisoning the demonstration context, without the need for fine-tuning the model." |
| Hijacking Large Language Models via Adversarial In-Context Learning | arXiv | 2023 | "This work introduces a novel transferable prompt injection attack against ICL, aiming to hijack LLMs to generate the target output or elicit harmful responses." |
| Data Poisoning for In-context Learning | NAACL | 2025 | "ICL performance can be significantly compromised by these attacks, highlighting the urgent need for improved defense mechanisms." |

## OWASP Classification

| OWASP ID | Name | Relevance |
|----------|------|-----------|
| LLM01:2025 | Prompt Injection | V-01, V-02, V-04, V-05, V-06, V-07, V-08 |
| LLM02:2025 | Sensitive Information Disclosure | V-03 |
| LLM05:2025 | Improper Output Handling | V-08 |
| LLM06:2025 | Excessive Agency | V-02, V-06 |
| LLM07:2025 | System Prompt Leakage | V-03 |

## MITRE ATLAS

- **AML.T0051 LLM Prompt Injection** — https://atlas.mitre.org/techniques/AML.T0051
- **26 CVEs mapped** — https://aithreatalert.com/reports/atlas-landscape/AML.T0051

## Downloaded Papers

1. `1_USENIX_Prompt_Injection_Benchmark.pdf` — USENIX Security 2024
2. `2_Prompt_Leakage_Multi_Turn.pdf` — EMNLP 2024
3. `3_ICLAttack_Backdoor.pdf` — EMNLP 2024
4. `4_ToolCommander_Tool_Injection.pdf` — NAACL 2025
5. `5_StructTransform_XML_Injection.pdf` — arXiv 2025
6. `6_ChatInject_Chat_Template_Injection.pdf` — arXiv 2025
7. `7_InjecAgent_Tool_Integrated.pdf` — arXiv 2024
8. `8_Hijacking_ICL.pdf` — arXiv 2023
9. `9_System_Prompt_Extraction_Survey.pdf` — arXiv 2025
10. `10_Prompt_Injection_Survey.pdf` — arXiv 2024
