# LLMXowl: Ontology Matching with Large Language Models

## Overview
LLMXowl is a framework for Ontology Matching (OM) that leverages Large Language Models through:
- Zero-shot prompting across three ontology representations
- Retrieval and matching modules
- Support for 20+ OM datasets across domains

## Key Features
- RAG (Retrieval Augmented Generation) approach
- Multiple LLM support (Mistral-7B, LLaMA-2, GPT-3.5, etc.)
- Flexible concept representations (C, CC, CP)
- Comprehensive evaluation framework
- State-of-the-art matching performance

## Installation
```bash
git clone https://github.com/MM-Aref/LLMXowl.git
cd LLMXowl
pip install -r requirements.txt
mv .env-example .env
