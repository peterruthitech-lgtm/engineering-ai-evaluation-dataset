
# Engineering AI Output Evaluation Dataset

**Applied engineering AI output evaluation dataset with correctness labels, error types, and technical review for AI data quality roles.**

---

## Overview

This repository contains a professionally curated dataset of AI-generated responses in the fields of **electronics, electrical engineering, embedded systems, power systems, and control systems**. Each response is carefully **evaluated and labeled** for correctness, error type, confidence, and human explanations.  

The project demonstrates applied engineering reasoning and AI evaluation skills, suitable for entry-level roles such as **AI data reviewer**, **AI quality analyst**, or **AI evaluation assistant**.

---

## Project Motivation

AI models can generate **plausible but incorrect outputs**, which can be dangerous in engineering contexts. This dataset:

- Provides **structured human evaluations** of AI responses  
- Highlights common **AI errors and reasoning gaps**  
- Demonstrates the ability to **audit and correct AI outputs**  

It is designed as a **portfolio project** to showcase both **engineering knowledge** and **AI evaluation expertise**.

---

## Dataset Details

The dataset is stored in `data/engineering_ai_output_evaluation.csv` and contains the following columns:

| Column | Description |
|--------|-------------|
| `sample_id` | Unique identifier for each AI response |
| `domain` | Engineering domain (electronics, electrical_engineering, embedded_systems, power_systems, control_systems) |
| `question` | Applied engineering question |
| `ai_model` | AI model generating the response (e.g., GPT-4, GPT-3.5) |
| `ai_response` | The AI-generated answer |
| `correctness_label` | Label: `correct`, `partially_correct`, `incorrect`, `misleading_or_unsafe` |
| `error_type` | Type of error if present (factual_error, reasoning_error, calculation_error, conceptual_misunderstanding, omission, unsafe_advice, none) |
| `confidence_level` | Confidence of the AI response (1–5) |
| `human_evaluation_explanation` | Detailed explanation of correctness and reasoning |
| `recommended_correction` | Suggestions for improving AI response |

---

## Labeling Guidelines

The labeling follows professional **AI evaluation standards**:

1. Read the question carefully and determine the expected correct answer  
2. Review AI response for correctness, reasoning, and potential errors  
3. Assign `correctness_label` and `error_type`  
4. Record AI confidence level  
5. Provide a detailed `human_evaluation_explanation` referencing applied engineering knowledge  
6. Optionally suggest `recommended_correction.`  

Full step-by-step instructions are in `docs/evaluation_guidelines.md`.

---

## Example Entries

| sample id | question | ai response | correctness_label | error type | human evaluation explanation |
|-----------|---------|-------------|-----------------|-----------|----------------------------|
| ENG-001 | A capacitor blocks DC but allows AC to pass. Explain why. | "Capacitors allow AC to pass because DC is blocked and AC flows freely." | partially correct | conceptual_misunderstanding, omission | AI is partially correct; it correctly identifies AC/DC behavior but omits capacitive reactance and frequency effects. |
| ENG-010 | Can you measure current in a high-voltage circuit with a standard multimeter? | "Yes, with caution." | misleading or unsafe | unsafe advice | AI gives dangerously unsafe advice; standard multimeters are not rated for high voltage/current. |

---

## Folder Structure

engineering AI evaluation dataset/

data/
    engineering AI output evaluation.csv
docs/
   evaluation guidelines.md
notebooks/       
   dataset analysis.ipynb
README.md
LICENSE
.gitignore


---

## Usage

1. Download the repository  
2. Open the CSV file in Excel, LibreOffice, or Python/pandas  
3. Explore AI responses and labels  
4. Use as a **portfolio reference** or **practice dataset for AI evaluation workflows**  

---

## Future Work

- Expand dataset to include **multi-model comparisons**  
- Include **real-world measurement data** for more applied evaluation  
- Develop scripts to **automate labeling consistency checks**  

---

## License

This project is licensed under the [MIT License](LICENSE).  

---

