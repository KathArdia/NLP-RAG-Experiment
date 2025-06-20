# Методы Retrieval-Augmented Generation (RAG): Экспериментальное исследование

**Автор:** Пономарев Дмитрий Валентинович  
**Проект для дисциплины:** Генеративные задачи в NLP, Томский государственный университет

---

## Описание

Данный проект посвящён исследованию различных стратегий Retrieval-Augmented Generation (RAG) на примере задачи генерации текстовых ответов с использованием моделей Nebius AI и анализа параметров чанкинга, топ-K и стратегий поиска.

- В ноутбуке `GEN_NLP_RAG_Ponomarev.ipynb` содержится полный эксперимент с кодом, метриками, сравнением стратегий (Simple RAG, Query Rewrite, Rerank) и автоматической оценкой качества.
- Итоговая статья находится в файле `NLP_RAG_Ponomarev_report.docx`.

## Состав репозитория

- `GEN_NLP_RAG_Ponomarev.ipynb` — Jupyter Notebook с кодом эксперимента
- `NLP_RAG_Ponomarev_report.docx` — финальная статья по результатам эксперимента
- `requirements.txt` — зависимости Python для запуска ноутбука

## Как запустить ноутбук

1. Откройте ноутбук через [Google Colab](https://colab.research.google.com/) или Jupyter Notebook.
2. Установите библиотеки из requirements.txt (в Colab можно просто запустить соответствующую ячейку).
3. Пропишите ваши ключи Nebius AI/OpenAI (если требуется).
4. Следуйте комментариям по коду.

## Краткие выводы

- Стратегия Rerank показала наивысшие метрики для данной задачи.
- Размер чанка 150, overlap 30 и top_k=3 оптимальны для точных ответов.
- Использование автоматической LLM-оценки облегчает сравнение конфигураций.

## Лицензия

MIT

---

