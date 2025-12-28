# 🔢 Tokenization in Large Language Models

## 📘 Overview
Tokenization is one of the most fundamental steps in any Large Language Model (LLM) pipeline.
Before a model can apply attention, generate embeddings, or predict text, raw language must first be converted into a numerical form.


Understanding tokenization helps explain many surprising behaviors of LLMs, including context limits, cost, and prompt sensitivity.

---

## ❓ What Is Tokenization?
Tokenization is the process of breaking raw text into smaller units called **tokens**.

A token can be:
- A full word  
- Part of a word (subword)  
- Punctuation  
- Symbols or special characters  

These tokens are then mapped to numbers so that neural networks can process them.

---

## 🏗️ Why Tokenization Exists
Neural networks operate on numbers, not text.

Tokenization exists to:
- Convert language into numerical form  
- Limit the size of the model’s vocabulary  
- Make training and inference computationally feasible  

Without tokenization, LLMs would not be able to scale to large datasets or long inputs.

---

## ⚙️ How Tokenization Is Used in LLMs
In an LLM pipeline:
1. Raw text is split into tokens  
2. Tokens are converted into token IDs (numbers)  
3. Token IDs are transformed into embeddings  
4. Transformers operate on these embeddings  

Every downstream process in an LLM depends on tokenization happening correctly.

---

## 🎯 Purpose of Tokenization
The purpose of tokenization is to:
- Standardize text input  
- Enable numerical representation of language  
- Balance expressiveness with efficiency  

Good tokenization allows models to handle:
- Different languages  
- Rare words  
- New or unseen text  

---

## ✅ What Tokenization Is Useful For
Tokenization enables:
- Defining the context window (token limits)  
- Controlling computational cost  
- Efficient training of large models  
- Consistent processing of diverse text inputs  

Many practical GenAI concerns — such as prompt length limits and pricing — are directly tied to token counts.

---

## ⚠️ Limitations of Tokenization
Tokenization has important limitations:

- It can split words in unintuitive ways  
- It does not preserve meaning by itself  
- Different languages produce different token counts  
- Formatting changes can affect token usage  

Because of this:
- Prompts may behave unexpectedly  
- Long inputs may be truncated  
- Small formatting changes can alter outputs  

---

## 🎯 Key Takeaway
> LLMs do not see words or sentences — they see tokens.

Tokenization is where language first becomes numbers, and its design has a direct impact on model behavior, cost, and reliability.

---

## 🧪 Exploration Note
This document is part of an ongoing exploration of Generative AI concepts, focusing on understanding foundational design choices before moving to higher-level system components.
