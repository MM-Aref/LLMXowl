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

```
from ontomap.ontology import MouseHumanOMDataset
from ontomap.base import BaseConfig
from ontomap.ontology_matchers import MistralLLMBertRAG

# Initialize configuration
config = BaseConfig(approach='rag').get_args(device='cuda')

# Load and process dataset
ontology = MouseHumanOMDataset().collect(root_dir="datasets")

# Generate matches
model = MistralLLMBertRAG(config.MistralBertRAG)
predicts = model.generate(input_data=encoded_inputs)
```

## Citation
```
@misc{giglou2024llms4om,
    title={LLMs4OM: Matching Ontologies with Large Language Models},
    author={Hamed Babaei Giglou and Jennifer D'Souza and Felix Engel and Sören Auer},
    year={2024},
    eprint={2404.10317},
    archivePrefix={arXiv}
}
```

