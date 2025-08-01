# 🧠 NCERT Grade 8 Science Structured Extraction using T5 LLM

This project demonstrates how to use **Large Language Models (LLMs)** — specifically `T5` — to extract well-structured, chapter-wise, topic-wise data from **NCERT Class 8 Science** textbooks in PDF format. It also includes automatic **JSON structuring**, **Excel generation**, a **study planner PDF**, and all supporting Python code.

---


## 📌 Problem Statement

The goal is to extract structured educational content that can support:
- Curriculum mapping
- Teaching plans
- AI chatbot integration
- Visual Knowledge Graph creation

---

## 🔍 What This Project Does

1. ✅ **Extracts structured data** from NCERT PDFs using T5-based LLM prompts.
2. 📂 Stores the output in clean **JSON** format.
3. 📊 Converts the structured data into a **readable Excel** file.
4. 📅 Generates a **15-day Study Planner** in PDF format.
5. 🤖 Uses reusable and robust **prompt engineering** for flexibility across chapters.

---

## 🛠️ Files in This Repository

| File Name | Description |
|-----------|-------------|
| `NCERT_Topic_Extraction.ipynb` | All code cells: prompt execution, parsing, JSON + Excel generation, PDF planner |
| `final_structured_with_topics.json` | Extracted topic-wise data from all chapters |
| `ncert_extracted_topics.xlsx` | Visualized output in Excel for validation |
| `ncert_study_planner_15_days.pdf` | Day-wise planner generated from topics |
| `prompts_used.txt` | The two universal prompts used: extraction + planner |

---

## 🧪 Techniques Used

- **Prompt Engineering**: Designed reusable, robust prompts compatible with any chapter structure.
- **LLM (T5)**: Used `valhalla/t5-base-qg-hl` model from Hugging Face for structured extraction.
- **Text Parsing**: Used regular expressions to separate chapters, topics, and subtopics.
- **Excel Automation**: Converted JSON into tabular format using `pandas` for readability.
- **Study Planner PDF**: Generated from JSON with day-wise topic distribution using `fpdf`.

---

## 📚 Chapters Processed

The following 4 NCERT chapters were used:
1. **Chapter 6** - Reproduction in Animals
2. **Chapter 7** - Reaching the Age of Adolescence
3. **Chapter 8** - Force and Pressure
4. **Chapter 13** - Light

---

## 🏗️ Dependencies

Install using pip:
```bash
pip install transformers torch fpdf pandas
