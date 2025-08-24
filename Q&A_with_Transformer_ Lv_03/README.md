# BERT Fine-tuning for Question Answering 

A comparative study fine-tuning BERT-Large and DistilBERT on the SQuAD v1.1 dataset for question answering tasks.

## Objectives

- Build a question answering system using transformer models
- Extract precise answer spans from context passages
- Compare performance and efficiency between BERT-Large and DistilBERT
- Evaluate using Exact Match (EM) and F1 Score metrics

## Models

**BERT-Large-uncased-whole-word-masking**
- Larger, more complex architecture
- Higher accuracy but greater computational requirements

**DistilBERT-base-uncased-distilled-squad**
- Compact, efficient model using knowledge distillation
- ~6x smaller than BERT while retaining ~97% performance
- Faster inference with minimal accuracy loss

## Methodology

1. **Environment Setup** - Install transformers, datasets, evaluate libraries
2. **Data Loading** - Load and partition SQuAD v1.1 dataset
3. **Model Initialization** - Initialize pre-trained models and tokenizers
4. **Preprocessing** - Tokenize contexts/questions, handle long sequences with stride, map answer spans
5. **Training** - Fine-tune both models using Hugging Face Trainer
6. **Evaluation** - Compute EM and F1 scores, qualitative testing

## Key Findings

**Performance vs Efficiency Trade-off**
- BERT-Large: Superior accuracy but higher computational cost
- DistilBERT: Competitive performance with significantly reduced resource requirements

**Knowledge Distillation Success**
- DistilBERT maintains high performance despite being much smaller
- Ideal for resource-constrained environments and fast inference needs

## Results

| Model | Exact Match (EM) | F1 Score |
|-------|------------------|----------|
| BERT-Large | 74.40% | 85.20% |
| DistilBERT | 73.60% | 83.82% |

## Quick Start

```bash
# Clone repository
git clone [repository_url]
cd [repository_name]

# Install dependencies
pip install transformers datasets evaluate torch

# Launch Jupyter
jupyter notebook

# Open qa_bert.ipynb and run all cells
```

## Conclusion

DistilBERT offers an excellent balance of performance and efficiency, making it suitable for production deployments where computational resources are limited while BERT-Large provides maximum accuracy for research applications.
