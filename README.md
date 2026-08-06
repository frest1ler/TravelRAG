# Tourist RAG: Интерактивный поисковик по достопримечательностям

> Retrieval-Augmented Generation (RAG) для поиска и интеллектуального обобщения информации о достопримечательностях российских городов.

---

# Описание

**Tourist RAG** — это проект, реализующий архитектуру **Retrieval-Augmented Generation (RAG)** для туристической информации. Система позволяет находить и обобщать сведения о памятниках архитектуры и достопримечательностях нескольких городов России (включая Владимир), сочетая современные методы векторного поиска и генерации текста.

В отличие от классического поиска по ключевым словам, проект сначала находит наиболее релевантные документы с помощью моделей эмбеддингов и ранжирования, а затем формирует краткий и информативный ответ на естественном языке.

---

# Ключевые возможности

- ✅ Семантический поиск по базе туристических объектов
- ✅ Retrieval-Augmented Generation (RAG)
- ✅ Векторный поиск на основе эмбеддингов
- ✅ Реранжирование результатов для повышения точности
- ✅ Генерация кратких и информативных ответов
- ✅ Поддержка запросов на русском языке
- ✅ Визуализация эмбеддингов и анализ качества поиска
- ✅ Простое масштабирование на новые города и достопримечательности

---

# Tech Stack

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-FFD21E?logo=huggingface&logoColor=black)
![Sentence Transformers](https://img.shields.io/badge/SentenceTransformers-E5E5E5)
![LangChain](https://img.shields.io/badge/LangChain-00A67E)
![ChromaDB](https://img.shields.io/badge/Chroma-VectorDB-7B61FF)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?logo=plotly&logoColor=white)

### Основные библиотеки

- Python
- PyTorch
- Hugging Face Transformers
- Sentence Transformers
- LangChain
- ChromaDB
- RAGatouille
- scikit-learn
- Pandas
- NumPy
- NLTK
- pymorphy2
- Plotly
- UMAP
- Matplotlib

---

# Getting Started

## Требования

- Linux Mint 21+
- Python 3.10+
- Git
- pip
- Jupyter Notebook / JupyterLab

---

## Установка

```bash
git clone https://github.com/<username>/tourist-rag.git

cd tourist-rag

python3 -m venv .venv

source .venv/bin/activate

pip install --upgrade pip

pip install -r requirements.txt
```

---

## Настройка `.env`

Если используются модели или сервисы Hugging Face:

```text
HF_TOKEN=your_huggingface_token
```

Создайте файл `.env` в корне проекта и добавьте необходимые переменные.

---

## Запуск

Запуск JupyterLab:

```bash
source .venv/bin/activate

jupyter lab
```

или Jupyter Notebook:

```bash
source .venv/bin/activate

jupyter notebook
```

После запуска откройте файл:

```text
hf_rag.ipynb
```

---

# Особенность проекта

Ключевой особенностью проекта является **гибридный конвейер Retrieval-Augmented Generation**, который объединяет:

1. Предобработку и нормализацию текстов.
2. Построение векторных представлений документов.
3. Семантический поиск релевантных объектов.
4. Реранжирование найденных результатов.
5. Генерацию итогового ответа языковой моделью.

Такой подход позволяет получать более точные ответы по туристическим объектам, чем традиционный поиск по ключевым словам.

---

# Структура проекта

```text
.
├── data/                  # Данные о достопримечательностях
├── hf_rag.ipynb           # Основной ноутбук проекта
├── requirements.txt       # Зависимости проекта
├── README.md
└── .env
```

---

# Выполнение

Для проверки работы выполните ноутбук полностью:

```bash
source .venv/bin/activate

jupyter notebook hf_rag.ipynb
```

---
