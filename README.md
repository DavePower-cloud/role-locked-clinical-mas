# A Role-Locked Multi-Agent LLM System for Clinical Dialogue: A Feasibility Study

This repository accompanies the manuscript:

**A Role-Locked Multi-Agent LLM System for Clinical Dialogue: A Feasibility Study**

submitted to *Intelligence-Based Medicine*.

## Overview

This study investigates the feasibility of a role-locked, multi-agent large language model (LLM) framework for generating clinically plausible and educationally usable simulated clinical dialogue.

The framework models a multi-party emergency department interaction using separate LLM agents representing a doctor, patient, and nurse. Each agent is assigned a defined conversational role and operates within explicit role constraints. Generated conversations are evaluated using both independent human assessment and an automated LLM-based evaluation framework.

The study also includes a single-agent comparator to examine whether role-specific multi-agent decomposition provides measurable advantages over generation of the complete clinical interaction by a single LLM.

## Reproducibility Materials

The accompanying **Supplementary Methods and Reproducibility Materials** document provides detailed information required to understand and reproduce the experimental framework, including:

- multi-agent system architecture and conversation workflow;
- exact role-specific prompts used for the doctor, patient, and nurse agents;
- model identifiers and generation configurations;
- role-guard rules, validation procedures, retry logic, and fallback behaviour;
- conversational context and turn-management procedures;
- single-agent comparator configuration and exact prompt;
- automated GPT-4o evaluation prompt, rubric, and structured output specification;
- statistical analysis methodology; and
- representative fully synthetic clinical conversations.

## Models

The multi-agent framework used the following models:

| Role | Model |
|---|---|
| Doctor | `gpt-4.1-mini-2025-04-14` |
| Patient | `claude-haiku-4-5-20251001` |
| Nurse | `gemini-3.1-flash-lite` |
| Automated evaluator | GPT-4o |
| Single-agent comparator | `claude-haiku-4-5-20251001` |

The use and configuration of these models are described in detail in the accompanying supplementary material.

## Repository Status

This repository is being developed as the public reproducibility archive accompanying the study.

The **Supplementary Methods and Reproducibility Materials** are currently available.

Additional study materials are being curated and documented for public release, including:

- study-specific source code;
- conversation-generation and evaluation notebooks;
- statistical analysis notebooks; and
- additional fully synthetic conversation data.

These materials will be added as reproducibility checks and documentation are completed.

## Data

All clinical conversations used in this study were generated synthetically.

**No real patient data, electronic health records, or patient-identifiable information were used in the generation or evaluation of the conversations.**

Representative synthetic conversations are provided in the supplementary material. Additional synthetic data will be added to this repository as part of the full reproducibility release.

## Supplementary Material

The supplementary material should be consulted alongside the manuscript for detailed implementation and reproducibility information.

**Supplementary Methods and Reproducibility Materials**  
*A Role-Locked Multi-Agent LLM System for Clinical Dialogue: A Feasibility Study*

## Citation

Citation information will be added following publication.

## Contact

Questions regarding the study or reproducibility materials should be directed to the corresponding author.

## Repository Development

This repository represents the research implementation evaluated in the accompanying manuscript. It is intended to support scientific transparency and reproducibility and should not be interpreted as a production clinical system or a validated clinical decision-support tool.
