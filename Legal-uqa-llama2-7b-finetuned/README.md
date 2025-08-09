# 🏛️ LEGAL-UQA: Llama-2 QLoRA Fine-tuning (Bilingual Legal Q&A)

This project fine-tunes the `NousResearch/Llama-2-7b-chat-hf` model into a specialized large language model for legal question-answering in both English and Urdu. Utilizing QLoRA with 4-bit NF4 quantization, it aims to be a powerful and resource-efficient AI assistant for the legal domain.

## ✨ Project Overview

The primary goal is to create an AI capable of producing accurate, contextually relevant, and linguistically appropriate legal responses. It serves as an invaluable tool for:

* **Bilingual Legal Research:** Assisting professionals with queries in English and Urdu.
* **Document Analysis:** Aiding in the understanding of legal texts.
* **Conversational Assistance:** Providing interactive, chat-based support for legal inquiries.

## 📊 Dataset

The project is built upon the **Legal-UQA Dataset**, a custom bilingual collection tailored for legal Q&A.

* **Source:** Available on Hugging Face Hub: `haroon-ahmad/legal-uqa-formatted`.
* **Content:** Contains parallel English and Urdu legal questions, contexts, and answers, derived from the Constitution of Pakistan.
* **Format:** Pre-processed into `Llama-2-chat`'s conversational prompt template (`<s>[INST]...[/INST]...</s>`) for optimal interaction.

## 🛠️ Techniques & Libraries Utilized

Efficient fine-tuning was achieved through:

* `bitsandbytes`: For **4-bit NF4 quantization**, significantly reducing model memory footprint.
* `PEFT` (QLoRA): Freezes most parameters, training only small adapters for efficiency and to prevent catastrophic forgetting.
* `Transformers`: Core library for model architecture and tokenizer.
* `Datasets`: For efficient data loading and processing.
* `TRL` (`SFTTrainer`): Streamlines supervised instruction fine-tuning.

## ⚙️ Training Process Highlights

The fine-tuning regimen focused on effectiveness and optimization:

1. **Prompt Token Masking**: Ensures the model learns to generate only the response.
2. **Learning Rate Scheduling**: Guides efficient model convergence.
3. **Mixed-Precision Training**: Enhances training speed and reduces memory.
4. **QLoRA Hyperparameter Tuning**: Optimized `lora_rank`, `lora_alpha`, and `lora_dropout` for performance.
5. **Progress Monitoring**: Tracked via validation loss and qualitative response assessments.

## 🎉 Outcome & Model Capabilities

The resulting **Legal-UQA Llama-2 QLoRA** model offers:

* **Bilingual Proficiency**: Seamless understanding and generation in English and Urdu.
* **Domain Expertise**: Strong grasp of legal terminology and concepts from constitutional law.
* **Conversational Fluency**: Maintains a helpful and intuitive chat experience.
* **Resource Efficiency**: Deployable on more accessible hardware due to QLoRA.

This model marks a significant step towards accessible and intelligent legal AI in multilingual contexts.

## 🔗 Resources

* **Training Dataset:** `haroon-ahmad/legal-uqa-formatted`
* **Final Fine-tuned Model:** `haroon-ahmad/urdu-legal-qa-pak`
