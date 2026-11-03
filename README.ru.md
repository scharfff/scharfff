<p align="center">
  <a href="https://t.me/pullubu"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram"></a>
  <a href="https://www.linkedin.com/in/liiilia/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://scholar.google.com/citations?user=1SYAk28AAAAJ"><img src="https://img.shields.io/badge/Google%20Scholar-4285F4?style=flat-square&logo=googlescholar&logoColor=white" alt="Google Scholar"></a>
  <a href="https://orcid.org/0009-0002-8954-8867"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID"></a>
  <a href="https://www.webofscience.com/wos/author/record/NZO-1576-2025"><img src="https://img.shields.io/badge/Web%20of%20Science-5E33BF?style=flat-square&logo=clarivate&logoColor=white" alt="Web of Science"></a>
</p>

<p align="left">
  <b>ML-инженер</b><br>
  Document AI и RAG-системы для технических и промышленных областей.
</p>


---
<p align="center">
  <a href="https://github.com/scharfff">English</a> · <b>Русский</b>
</p>

Проектирую системы анализа документов на базе LLM: RAG по нормативной документации, OCR-пайплайны, извлечение структурированных данных с валидацией, дообученные BERT-подобные модели для NER и классификации. Большая часть этой работы шла на закрытых корпоративных документах, со сравнением локальных моделей и облачных провайдеров.

По первому образованию я инженер-строитель (BIM), поэтому технические документы знаю изнутри. Ещё преподаю Python, информатику и математику абитуриентам в СПбПУ и занимаюсь исследованиями в NLP.

<details>
<summary><b>Проекты</b></summary>

&nbsp;

### DocuLex: сервис анализа договоров (закрытый код)

- **Задача.** Разбор договора вручную занимал около 15 минут.
- **Архитектура.** PDF, DOCX и сканы проходят OCR-пайплайн. Структурированное извлечение возвращает 17 полей с валидацией по схеме Pydantic, затем формируются отчёты PDF и XLSX. Интерфейс: Telegram-бот. Развёрнут в Docker на Amvera.
- **Результат.** Я сделала его в «Синтезе» по собственной инициативе. Разбор занимает около 5 минут вместо примерно 15, сервис до сих пор используется в компании.

### RAG по технической нормативной документации в «Синтезе» (закрытый код)

- **Задача.** Поиск по техническим регламентам (ПУЭ, ПТЭЭП, ГОСТ, РД) в закрытом корпоративном корпусе примерно из 300 документов.
- **Стек.** LangChain, ChromaDB, эмбеддинги ruBERT, сервис на FastAPI, Langfuse для трейсинга, Docker.

### [electrolabbot](https://github.com/scharfff/electrolabbot): открытый RAG-ассистент по нормам электротехнических испытаний

- **Задача.** Работающая RAG-система для электротехнических испытаний только на открытых нормах и синтетических отчётах, без приватных данных.
- **Архитектура.** Открытые нормы (ПУЭ, ПТЭЭП, СП, ГОСТ, РД) и 15 обезличенных синтетических отчётов, сгенерированных скриптом. Эмбеддинги ruBERT и хранилище Chroma с HNSW-индексом работают локально, есть память диалога. LLM вызывается через Hugging Face Inference API. Трейсинг в Langfuse опционален. Интерфейсы: Streamlit, REST API на FastAPI и CLI. В репозитории есть конфиги Docker и Amvera.
- **Компромисс.** Используется бесплатный тариф облачной LLM. В README указаны лимит 30 000 запросов в месяц и задержка от 2 до 5 секунд, а также способы смягчения: кеширование и асинхронная обработка.

### [TapKeys](https://github.com/scharfff/tapkeys): жесты трекпада в сочетания клавиш на macOS (Swift, MIT)

- **Архитектура.** Касания приходят из приватного `MultitouchSupport.framework` Apple, который загружается в рантайме через `dlsym`. `CGEvent` tap перехватывает только клики тремя или четырьмя пальцами, у которых есть привязка. Буквенные сочетания следуют текущей раскладке, в том числе AZERTY, Dvorak и русской.
- **Ограничения.** Приватные API могут измениться между релизами macOS. Приложение проверено на macOS 15 (Intel), подписано ad hoc и не нотаризовано. Это указано в README вместе с обходными путями.
- **Релизный пайплайн.** CI запускается на каждый pull request и каждый push в main. Тег версии собирает универсальный бинарник, zip и DMG, а сборка проверяет подпись и обе архитектуры и прогоняет самотест из DMG. Релиз создаётся как черновик, контрольные суммы загруженных файлов сверяются с `SHA256SUMS`, затем он публикуется и обновляется Homebrew cask. v0.2.0 стала первым стабильным релизом: `brew install --cask scharfff/tap/tapkeys`.

### [spbpu-inf-course](https://github.com/scharfff/spbpu-inf-course): веб-учебник по ЕГЭ по информатике 2027

- **Архитектура.** Веб-приложение на Astro, которое собирается и выкладывается через GitHub Actions на GitHub Pages. Материалы лежат в папках по заданиям, решения на Python. Прошлый год хранится в отдельной ветке (2026), а в README описан проект спецификации 2027 года: 27 заданий и 29 первичных баллов.
- **Результат.** Ядро моей образовательной платформы и материал для моих занятий в СПбПУ. [Открыть веб-приложение](https://scharfff.github.io/spbpu-inf-course/).

### [mailrucloud](https://github.com/scharfff/mailrucloud): неофициальный CLI для Mail.ru Облака (PyPI)

- **Архитектура.** Python и Click поверх WebDAV. В версии 1.1.0 я заменила устаревший REST API на WebDAV. Многопоточная загрузка (по умолчанию 4 потока) появилась в 1.4.2, и по данным [CHANGELOG](https://github.com/scharfff/mailrucloud/blob/master/CHANGELOG.md) синхронизация стала быстрее от 4 до 8 раз.
- **Инженерия.** Тесты на pytest, CI на Python 3.10 и 3.11, релизы уходят на [PyPI](https://pypi.org/project/mailru-cloud-cli/) через publish-workflow: `pip install mailru-cloud-cli`.

### Исследования

Магистерское исследование лингвистических маркеров типа личности в текстах: [MBTI-LSTM](https://github.com/scharfff/MBTI-LSTM), BiLSTM-классификатор на PyTorch. Также участвовала в исследовании для системы распознавания птиц на основе свёрточных сетей по снимкам камер наблюдения.

</details>

<details>
<summary><b>Опыт</b></summary>

&nbsp;

- **С 2025 по настоящее время.** Преподаватель (совместительство), СПбПУ, центр работы с абитуриентами. Собственный курс и веб-платформа для него.
- **С 2024 по 2025.** ML-инженер, «Синтез», команда IT-инфраструктуры. RAG-система, DocuLex, дообученные BERT-подобные модели для NER и классификации протоколов испытаний, дообученная модель Hugging Face для суммаризации документации электролаборатории.
- **С 2023 по 2024.** Аналитик-разработчик, «Синтез», команда IT-инфраструктуры. Сравнение локальных моделей с облачными провайдерами (OpenAI, Hugging Face, Сбер, Яндекс), A/B-тесты ML- и AI-решений с постанализом.
- **С 2022 по 2024.** Инженер-исследователь (совместительство), СибГИУ, кафедра информационных технологий. Исследования LSTM- и BiLSTM-классификатора.
- **С 2022 по 2023.** Стажёр-аналитик, «Синтез». ETL-процессы, дашборды, оцифровка технической документации по ГОСТ.

</details>

<details>
<summary><b>Публикации</b></summary>

&nbsp;

Публикации на русском языке, вышли под именем Самойлова Л. (фамилия теперь Scharf). Варианты написания связаны в Google Scholar. Web of Science ResearcherID: [NZO-1576-2025](https://www.webofscience.com/wos/author/record/NZO-1576-2025).

1. Самойлова Л., Гулевич Т. М. Применение искусственной нейронной сети с пятифакторной моделью личности для подбора персонала. Наука и молодёжь: проблемы, поиски, решения: труды Всероссийской научной конференции. Вып. 28. Ч. II. СибГИУ, 2024.
2. Самойлова Л., Даниловский В. М. Прогнозирование личностных характеристик MBTI с использованием рекуррентной нейронной сети LSTM и текстовых данных социальных сетей. Вестник науки. 2024. Т. 4, № 6 (75). С. 1176 по 1184. [Текст на КиберЛенинке](https://cyberleninka.ru/article/n/prognozirovanie-lichnostnyh-harakteristik-mbti-s-ispolzovaniem-rekurrentnoy-neyronnoy-seti-lstm-i-tekstovyh-dannyh-sotsialnyh-setey). Код: [MBTI-LSTM](https://github.com/scharfff/MBTI-LSTM).
3. Самойлова Л., Даниловский В. М. Интеллектуальная система распознавания птиц в видеонаблюдении на основе свёрточных нейронных сетей. Вестник науки. 2024. Т. 2, № 11 (80). С. 1149 по 1159. [Текст на КиберЛенинке](https://cyberleninka.ru/article/n/intellektualnaya-sistema-raspoznavaniya-ptits-v-videonablyudenii-na-osnove-svertochnyh-neyronnyh-setey)

</details>

<details>
<summary><b>Образование</b></summary>

&nbsp;

- Магистратура, «Информационные системы и технологии» (профиль «Интеллектуальные системы и технологии»), СибГИУ, с 2022 по 2024.
- Бакалавриат, «Промышленное и гражданское строительство» (BIM), СибГИУ, с 2018 по 2022.
- Английский: B2.

</details>

<details>
<summary><b>Стек</b></summary>

&nbsp;

- **ML:** Python, PyTorch, Hugging Face Transformers, дообучение (LoRA, PEFT), vLLM, Ollama
- **LLM и RAG:** LangChain, LlamaIndex, Chroma, Qdrant, Langfuse, PaddleOCR, Pydantic
- **Сервисы:** FastAPI, Docker, PostgreSQL, Linux, Git, GitHub Actions, Yandex Cloud, Cloud.ru, Amvera
- **Приложения:** Swift (TapKeys)

</details>
