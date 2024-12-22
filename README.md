# Next-Gen Dialogue Summarization Comparison

This repository contains experiments comparing different approaches to dialogue summarization using the FLAN-T5 model. The project evaluates zero-shot learning, few-shot learning, full fine-tuning, and PEFT (Parameter Efficient Fine-Tuning) methods, measuring performance using ROUGE metrics.

## Project Overview

The project explores various methods of adapting the FLAN-T5 model for dialogue summarization tasks:

1. **Zero-shot Learning**: Testing the model's ability to summarize dialogues without any task-specific training
2. **Few-shot Learning**: Using in-context examples to guide the model's summarization
3. **Full Fine-tuning**: Traditional fine-tuning of the entire model
4. **PEFT**: Parameter-efficient fine-tuning approach

## Repository Structure

```
.
│── Project.ipynb
│── dialogue-summary-training-results.csv
└── README.md
```

## Dataset

The dataset contains three columns comparing different summarization approaches:
- Human-written reference summaries
- Original model outputs
- Instruct model outputs
- PEFT model outputs

## Methods

### Zero-shot Learning
- Direct use of FLAN-T5 without any task-specific training
- Testing the model's inherent ability to understand and execute summarization tasks

### Few-shot Learning
- Providing the model with examples during inference
- Testing the model's ability to learn from in-context examples

### Full Fine-tuning
- Traditional fine-tuning of the entire FLAN-T5 model
- Adapting all model parameters to the summarization task

### PEFT (Parameter Efficient Fine-tuning)
- Efficient adaptation using parameter-efficient methods
- Reducing computational resources while maintaining performance

## Evaluation

The project uses ROUGE metrics for evaluation:
- ROUGE-1: Unigram overlap
- ROUGE-2: Bigram overlap
- ROUGE-L: Longest Common Subsequence

## Results
![Screenshot 2024-12-10 211122](https://github.com/user-attachments/assets/11b44a98-6b57-4f47-9f2d-503df74dd1af)

![Screenshot 2024-12-10 211218](https://github.com/user-attachments/assets/2fc6a3b1-840c-4e1a-b83c-9ef08efc69de)

![Screenshot 2024-12-10 211230](https://github.com/user-attachments/assets/bd230e33-de44-4f6e-a22b-8b63f4951994)

![Screenshot 2024-12-10 204922](https://github.com/user-attachments/assets/fdd2dee6-fb3b-423a-8f57-f5e4d1e80c76)

![Screenshot 2024-12-10 205014](https://github.com/user-attachments/assets/5dd82a8b-6157-42b7-ac2b-79d19ebd3e5d)

![Screenshot 2024-12-10 205432](https://github.com/user-attachments/assets/0fcf2acc-5c29-4c46-9054-f3d43a77117a)

![Screenshot 2024-12-10 205637](https://github.com/user-attachments/assets/e9d9a0aa-3f77-465c-a0d5-cdc9cd0dcd7e)

![Screenshot 2024-12-10 205749](https://github.com/user-attachments/assets/b2d0c607-d1ce-4396-b6c9-d06c7b5a4572)

![Screenshot 2024-12-10 205918](https://github.com/user-attachments/assets/0313bfd2-2373-43ae-800e-fef1e84ed8f7)

![Screenshot 2024-12-10 210141](https://github.com/user-attachments/assets/058fea43-32db-4f9d-bc5c-adca476c34e5)

![Screenshot 2024-12-10 210622](https://github.com/user-attachments/assets/0fce5c39-4828-4c23-b3dd-bf3b4147f845)

![Screenshot 2024-12-10 210850](https://github.com/user-attachments/assets/dfe3e785-a495-4f35-84cd-fad4ed48d9a4)

![Screenshot 2024-12-10 210922](https://github.com/user-attachments/assets/11e8eed5-fa7a-40cd-81f8-f81e031257a5)

## Requirements

- Python 3.8+
- PyTorch
- Transformers
- PEFT
- datasets
- rouge-score
- pandas
- numpy

## License

Apache License

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
