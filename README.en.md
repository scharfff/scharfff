<h1 align="center">Lilia Scharf</h1>

<p align="center">
  <b>ML engineer and researcher</b> · NLP · LLM · RAG · Document AI<br>
  <sub>Technical and industrial domains · closed corporate environments · Saint Petersburg</sub>
</p>

<p align="center">
  <a href="https://github.com/scharfff">Русский</a> &nbsp;·&nbsp; <b>English</b>
</p>

<p align="center">
  <a href="https://t.me/pullubu"><img src="https://img.shields.io/badge/Telegram-@pullubu-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram"></a>
  <a href="mailto:s.liiilia@mail.ru"><img src="https://img.shields.io/badge/Email-s.liiilia@mail.ru-EA4335?style=flat-square&logo=maildotru&logoColor=white" alt="Email"></a>
  <a href="https://www.linkedin.com/in/liiilia/"><img src="https://img.shields.io/badge/LinkedIn-liiilia-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://www.kaggle.com/lilyscharf"><img src="https://img.shields.io/badge/Kaggle-lilyscharf-20BEFF?style=flat-square&logo=kaggle&logoColor=white" alt="Kaggle"></a>
</p>
<p align="center">
  <a href="https://orcid.org/0009-0002-8954-8867"><img src="https://img.shields.io/badge/ORCID-0009--0002--8954--8867-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID"></a>
  <a href="https://scholar.google.com/citations?user=1SYAk28AAAAJ"><img src="https://img.shields.io/badge/Google%20Scholar-profile-4285F4?style=flat-square&logo=googlescholar&logoColor=white" alt="Google Scholar"></a>
  <a href="https://www.webofscience.com/wos/author/record/NZO-1576-2025"><img src="https://img.shields.io/badge/Web%20of%20Science-NZO--1576--2025-5E33BF?style=flat-square&logo=clarivate&logoColor=white" alt="Web of Science ResearcherID"></a>
  <a href="https://researchid.co/sliiilia"><img src="https://img.shields.io/badge/ResearchID-sliiilia-00CCBB?style=flat-square" alt="ResearchID"></a>
</p>

---

## About

I build LLM-based document analysis systems for technical and industrial domains: RAG search over regulatory documents, OCR pipelines, structured extraction, and fine-tuning of BERT-like models for NER and classification. I work where data cannot go to the cloud: closed corporate environments, local models, hybrid architectures.

Alongside engineering I do NLP research (linguistic features in text) and teach Python, computer science and mathematics to university applicants at SPbPU. My first degree is in civil engineering (BIM), so technical documents are a domain I know from the inside.

**Now:** teaching at SPbPU, developing an educational platform and preparing for PhD admission in 2027 (AI and machine learning).

---

## Publications

All papers were published in Russian under the surname **Samoilova L.** (now Scharf); the name variants are linked in ORCID, Google Scholar and ResearchID.

1. Samoilova L., Gulevich T. M. **Application of an artificial neural network with the Big Five personality model to personnel selection** // Proc. All-Russian Conf. "Science and Youth: Problems, Searches, Solutions", iss. 28, part II. Novokuznetsk: SibSIU, 2024.
2. Samoilova L., Danilovsky V. M. **Prediction of Personal Characteristics MBTI Using Recurrent Neural Network LSTM and Text Data of Social Networks** // Vestnik nauki. 2024. Vol. 4, no. 6 (75). Pp. 1176–1184. [Full text](https://cyberleninka.ru/article/n/prognozirovanie-lichnostnyh-harakteristik-mbti-s-ispolzovaniem-rekurrentnoy-neyronnoy-seti-lstm-i-tekstovyh-dannyh-sotsialnyh-setey) · code: [MBTI-LSTM](https://github.com/scharfff/MBTI-LSTM)
3. Samoilova L., Danilovsky V. M. **Intelligent Bird Recognition System in Video Surveillance Based on Convolutional Neural Networks** // Vestnik nauki. 2024. Vol. 2, no. 11 (80). Pp. 1149–1159. [Full text](https://cyberleninka.ru/article/n/intellektualnaya-sistema-raspoznavaniya-ptits-v-videonablyudenii-na-osnove-svertochnyh-neyronnyh-setey)

Google Scholar as of 27 Oct 2026: 5 citations · h-index 1.

---

## Selected projects

| Project | What it is | Stack and links |
|---|---|---|
| **[spbpu-inf-course](https://github.com/scharfff/spbpu-inf-course)** | Web textbook and course for the Russian computer science state exam, built for SPbPU applicants: theory, walkthroughs of every exam task, Python solutions, progress tracker. The core of the educational platform (in Russian) | Astro · Python · GitHub Actions → GitHub Pages · [open](https://scharfff.github.io/spbpu-inf-course/) |
| **[electrolabbot](https://github.com/scharfff/electrolabbot)** | Open RAG assistant for electrical testing standards (PUE, PTEEP, SP, GOST, RD): public standards and anonymized synthetic reports; Streamlit UI, REST API and CLI | ruBERT · Chroma · LangChain · Langfuse · FastAPI · Docker |
| **DocuLex** | Contract analysis service: PDF/DOCX and scans → OCR → extraction of 17 fields with validation (Pydantic) → PDF and XLSX reports, Telegram bot. Contract review takes about 5 minutes instead of 15 by hand. Built by me at Sintez on my own initiative and still used inside the company. Closed source | OCR · structured extraction · Pydantic · FastAPI · Docker |
| **[mailru-cloud-cli](https://github.com/scharfff/mailrucloud)** | CLI client for Mail.ru Cloud over WebDAV: upload, download, directory sync. Multithreaded upload sped up sync 4–8x ([CHANGELOG, v1.4.2](https://github.com/scharfff/mailrucloud/blob/master/CHANGELOG.md)) | `pip install mailru-cloud-cli` · [PyPI](https://pypi.org/project/mailru-cloud-cli/) · pytest · GitHub Actions (CI on Python 3.10 and 3.11, releases) |
| **[MBTI-LSTM](https://github.com/scharfff/MBTI-LSTM)** | Master's research project: an LSTM/BiLSTM classifier of personality-type features from text. Metrics and limitations are described in the repository README | PyTorch · BiLSTM · NLP |
| **[linux-tools-documentation](https://github.com/scharfff/linux-tools-documentation)** | Scripts and notes for Debian / Ubuntu / Astra Linux administration: sync process monitoring, notifications | Bash · cron · systemd |

<!-- Demo: uncomment when the servers are back.
| Demo | Link |
|---|---|
| electrolabbot (RAG over electrical standards) | https://electrolabbot.ru |
| DocuLex (contract analysis) | https://doculex.ru |
-->

---

## Experience

| Period | Role | What I did |
|---|---|---|
| 2025 – present | Lecturer (part-time), SPbPU, applicant outreach center | Own course and a platform for it; classes in Python, computer science and mathematics for applicants |
| 2024 – 2025 | ML Engineer, Sintez (IT infrastructure; company of about 30 people) | RAG system for search over technical documentation (PUE, PTEEP, GOST, RD), closed corpus of about 300 documents; DocuLex contract analysis service; fine-tuning of BERT-like models for NER and classification of technical test protocols; fine-tuning of an HF model for summarizing electrical-lab documentation |
| 2023 – 2024 | Analyst-developer, Sintez | Benchmarking local models against cloud providers (OpenAI, Hugging Face, Sber, Yandex); A/B tests of ML and AI solutions, post-analysis, reports; processing of electrical measurement lab data; access control infrastructure administration (Bolid, Orion Pro) |
| 2022 – 2024 | Research engineer (part-time), SibSIU | Linguistic markers of personality type in texts, LSTM classifier, corpus preprocessing pipelines; research for a CNN-based bird recognition system; a journal paper and conference proceedings |
| 2022 – 2023 | Analyst intern, Sintez | ETL processes, dashboards, digitizing technical documentation per GOST |

## Education

- **MSc**, Siberian State Industrial University (SibSIU), 2022–2024 — 09.04.02 Information Systems and Technologies, track "Intelligent Systems and Technologies"
- **BSc**, SibSIU, 2018–2022 — Industrial and Civil Engineering, information modeling and BIM
- English: B2

---

## Stack

**Language and ML:** Python · PyTorch · NumPy · Pandas · SciPy · Pydantic · Hugging Face Transformers · fine-tuning (LoRA / PEFT)

**LLM and RAG:** LLM APIs · vLLM · Ollama · LangChain · LlamaIndex · embeddings · Qdrant / Chroma · Langfuse · PaddleOCR

**Services and infrastructure:** FastAPI · Docker · PostgreSQL · Linux (Debian / Ubuntu / Astra) · Git · GitHub Actions · Yandex Cloud · Cloud.ru · Amvera

---

<p align="center">
  Contact: <a href="https://t.me/pullubu">Telegram @pullubu</a> (preferred) · <a href="mailto:s.liiilia@mail.ru">s.liiilia@mail.ru</a>
</p>
