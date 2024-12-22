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

![Screenshot 2024-12-10 204922](https://github.com/user-attachments/assets/e6446f7d-9380-4f06-9e34-fe3c35ab485c)

![Screenshot 2024-12-10 205014](https://github.com/user-attachments/assets/f76aa176-7a90-4c87-917f-aee0ca7ce648)

![Screenshot 2024-12-10 205432](https://github.com/user-attachments/assets/a175c2a9-2057-4a8c-9053-2abe36fcf8ab)

![Screenshot 2024-12-10 205637](https://github.com/user-attachments/assets/46522d2c-8188-41aa-aa38-1bd70cf8e9df)

![Screenshot 2024-12-10 205749](https://github.com/user-attachments/assets/663d825c-a89f-4a37-a41a-47aed0b53859)

![Screenshot 2024-12-10 205918](https://github.com/user-attachments/assets/79bc7009-98aa-4cd9-8005-d0d02e8c06d1)

![Screenshot 2024-12-10 210141](https://github.com/user-attachments/assets/e2764b11-1454-4a2f-95e2-78073ac7e075)

![Screenshot 2024-12-10 210622](https://github.com/user-attachments/assets/1bd08bf1-b543-444e-a0f7-8f67c8de74d4)

![Screenshot 2024-12-10 210850](https://github.com/user-attachments/assets/946b0c0f-7ccc-4fec-876b-314fcca7a5cf)

![Screenshot 2024-12-10 210922](https://github.com/user-attachments/assets/87e5be7d-c259-4ba0-b207-2045581423b1)

![Screenshot 2024-12-10 211122](https://github.com/user-attachments/assets/b3da38be-fec3-4a4e-9f61-217c44c38835)

![Screenshot 2024-12-10 211218](https://github.com/user-attachments/assets/e40e175b-4d14-44bb-9af6-9cb277b1cf96)

![Screenshot 2024-12-10 211230](https://github.com/user-attachments/assets/7322f535-7917-41a0-97b9-5556b1bc1954)


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
