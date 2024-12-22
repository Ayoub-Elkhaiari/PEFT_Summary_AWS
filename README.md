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

![Screenshot 2024-12-10 211218](https://github.com/user-attachments/assets/72ae57b7-e129-40a9-ac41-17ec407b6423)

![Screenshot 2024-12-10 211230](https://github.com/user-attachments/assets/b0e84a3a-3c48-40bf-92bc-938f0c3ea1bc)

![Screenshot 2024-12-20 235726](https://github.com/user-attachments/assets/2fb09c51-8509-49ff-8698-0f79c3124334)

![Screenshot 2024-12-10 204922](https://github.com/user-attachments/assets/c0694da3-5247-437e-b095-13f945a01578)

![Screenshot 2024-12-10 205014](https://github.com/user-attachments/assets/5a7ceda0-1ab8-42b2-a820-851069eae3aa)

![Screenshot 2024-12-10 205432](https://github.com/user-attachments/assets/81546e38-731b-455c-be4f-f01f56c9d942)

![Screenshot 2024-12-10 205637](https://github.com/user-attachments/assets/e1b26505-3420-4f6d-9c24-cb25b025b688)

![Screenshot 2024-12-10 205749](https://github.com/user-attachments/assets/8ac7575d-82a7-4d91-90a0-0b88630680d8)

![Screenshot 2024-12-10 205918](https://github.com/user-attachments/assets/056010dc-1f47-46e3-9d21-3703b27d1b2e)

![Screenshot 2024-12-10 210110](https://github.com/user-attachments/assets/4022ecaf-83dd-4e04-9a78-8177385e1454)

![Screenshot 2024-12-10 210141](https://github.com/user-attachments/assets/de93e258-ffa9-478f-a536-5225c383afb5)

![Screenshot 2024-12-10 210622](https://github.com/user-attachments/assets/15f19df1-3cf9-4330-b0a9-9a3f49d49a56)

![Screenshot 2024-12-10 210850](https://github.com/user-attachments/assets/6f448c52-c6e9-47f5-8c89-818922704ba4)

![Screenshot 2024-12-10 210922](https://github.com/user-attachments/assets/069b9398-3cd5-4305-b610-c296653721b3)

![Screenshot 2024-12-10 211122](https://github.com/user-attachments/assets/aae89e8e-429d-4dad-8963-578eddd5f198)

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
