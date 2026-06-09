<h1 align="center">Лилия Самойлова</h1>
<p align="center">
  <b>ML&nbsp;Engineer</b> · LLM-интеграции · RAG&nbsp;· Document-AI для технических и промышленных доменов
  <br>
  <sub>Санкт-Петербург · от прототипа до прода · закрытые корпоративные контуры</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/liiilia/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://t.me/mueqee"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=flat&logo=telegram&logoColor=white" alt="Telegram"></a>
  <a href="https://researchid.co/s.liiilia"><img src="https://img.shields.io/badge/ResearchID-00CCBB?style=flat&logo=orcid&logoColor=white" alt="ResearchID"></a>
  <a href="mailto:mueqee@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

## О себе

Проектирую и довожу до прода системы анализа документов на базе LLM: RAG-поиск по нормативной документации, OCR-пайплайны, structured extraction, дообучение BERT-подобных моделей под NER и классификацию. Работаю там, где данные нельзя отдать в облако - закрытые контуры, локальные модели, гибридные архитектуры.

Мне интересно превращать исследовательскую идею в работающий продукт: от гипотезы и эксперимента до сервиса, которым реально пользуются. Параллельно веду линию в NLP (анализ неявных лингвистических признаков в текстах) и преподаю Python и математику в СПбПУ. Сейчас ищу позицию **ML / LLM / NLP Engineer** и научную группу для PhD по направлению *искусственный интеллект и машинное обучение*.

---

## Живые демо

| Проект | Что это | Ссылка |
|---|---|---|
| **electrolabbot** | RAG-ассистент по нормам электротехнических испытаний (ПУЭ, ПТЭЭП, ГОСТ) | [electrolabbot.ru](https://electrolabbot.ru) |
| **DocuLex** | Анализ договоров: мультиформатный ввод PDF/DOCX, OCR, structured extraction, отчёты | [doculex.ru](https://doculex.ru) |
| **Курс для абитуриентов** | Подготовка к ЕГЭ по информатике: теория, разборы, решения на Python | [scharfff.github.io/spbpu-inf-course](https://scharfff.github.io/spbpu-inf-course/) |

---

## Стек

**Языки и ядро:** Python · PyTorch · NumPy · Pandas · SciPy · Pydantic
**LLM / NLP:** Hugging Face Transformers · fine-tuning (LoRA / PEFT) · ruBERT · LLM APIs · vLLM · Ollama
**RAG:** LangChain · LlamaIndex · embeddings · vector DB (Qdrant / Chroma) · Langfuse · PaddleOCR
**Сервис и инфра:** FastAPI · Docker · PostgreSQL · Linux (Debian / Ubuntu / Astra) · Git · CI/CD (GitHub Actions)
**Облака:** Yandex Cloud · cloud.ru · Amvera

---

## Избранные проекты

### electrolabbot RAG-ассистент для энергетики и промышленности
Поиск и интерпретация по нормативной базе электротехнических испытаний (ПУЭ, ПТЭЭП, СП, ГОСТ, РД) на **полностью открытых данных**. Помогает находить нормы, трактовать результаты измерений и заполнять протоколы.
`ruBERT embeddings` · `Chroma (HNSW)` · `Langfuse трейсинг` · `FastAPI + Streamlit + CLI` · `Docker`
→ демо: [electrolabbot.ru](https://electrolabbot.ru) · код: [github.com/scharfff/electrolabbot](https://github.com/scharfff/electrolabbot)

### DocuLex анализ договоров с LLM
Сервис извлечения структурированных данных из договоров: мультиформатный ввод PDF/DOCX, OCR-пайплайн, structured extraction 17 полей (Pydantic), генерация отчётов PDF и XLSX, Telegram-бот. Деплой через Docker.
`OCR` · `structured extraction` · `Pydantic` · `FastAPI` · `Docker`
→ демо: [doculex.ru](https://doculex.ru)

### mailru-cloud-cli опубликованный пакет на PyPI
CLI-клиент Mail.ru Облака через WebDAV: загрузка, скачивание, одно/двусторонняя синхронизация каталогов. Реальные пользователи, релизный цикл, тесты и CI.
`pip install mailru-cloud-cli` · `WebDAV` · `pytest` · `GitHub Actions` · `PyPI release`
→ [github.com/scharfff/mailrucloud](https://github.com/scharfff/mailrucloud) · [PyPI](https://pypi.org/project/mailru-cloud-cli/)

### MBTI-LSTM исследование, предсказание психотипа по тексту
BiLSTM-классификатор, извлекающий косвенные признаки личности (стиль, лексика, синтаксис) из текстов. Основа магистерской диссертации; по теме опубликованы статьи в РИНЦ.
`PyTorch` · `BiLSTM (128→64)` · `NLP preprocessing` · `research`
→ [github.com/scharfff/MBTI-LSTM](https://github.com/scharfff/MBTI-LSTM)

### linux-tools-documentation автоматизация и мониторинг в Linux
Коллекция shell-скриптов и документации для Debian / Ubuntu / Astra Linux: мониторинг процессов синхронизации, уведомления, типовые задачи администрирования.
`Bash` · `cron` · `systemd` · `Astra Linux`
→ [github.com/scharfff/linux-tools-documentation](https://github.com/scharfff/linux-tools-documentation)

---

## Опыт

| Период | Роль | Чем занималась |
|---|---|---|
| 2025 – 2026 | Преподаватель, СПбПУ | Курсы Python, информатики и профильной математики для абитуриентов |
| 2024 – 2025 | ML Engineer, «Синтез» | RAG-система по техдокументации (LangChain, ChromaDB, ruBERT, Langfuse, FastAPI); сервис анализа договоров (OCR, structured extraction 17 полей, отчёты PDF/XLSX, Telegram-бот); дообучение BERT под NER и суммаризацию |
| 2023 – 2024 | Аналитик-разработчик, «Синтез» | Подбор и бенчмаркинг локальных (Ollama) и облачных (OpenAI, HF, Sber, Yandex) моделей; AB-тесты ML/AI-решений, расчёт метрик |
| 2022 – 2024 | Инженер-исследователь, СибГИУ | Лингвистические паттерны MBTI в текстах; LSTM-классификатор; пайплайны предобработки корпусов. 2 публикации |

---

## Образование и наука

- **Магистратура**, СибГИУ интеллектуальные системы и технологии (2024). Диссертация: программный модуль на LSTM для анализа неявных сущностей в тексте и их корреляции с психотипами.
- **2 публикации** (РИНЦ) по теме психолингвистического анализа текстов.
- Профиль исследователя: [researchid.co/s.liiilia](https://researchid.co/s.liiilia)

---

## Сейчас в фокусе

- Открыта к позициям **ML / LLM / NLP Engineer** в Санкт-Петербурге, включая research-роли в лабораториях
- Готовлюсь к поступлению в аспирантуру по направлению *ИИ и машинное обучение*
- Углубляюсь в RAG-архитектуры для промышленных доменов и эффективный fine-tuning LLM

Связаться: [Telegram @mueqee](https://t.me/mueqee) (предпочтительно) · [LinkedIn](https://www.linkedin.com/in/liiilia/) · mueqee@gmail.com
