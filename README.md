# Ключевые статьи в области LLM reasoning - отчет

## 1. Как задана область?

Использован концепт [LLM Reasoning в OpenAlex](https://openalex.org/keywords/llm-reasoning). Получилось около **1000 статей**.

## 2. Что считать ключевой статьей

Использовано определение **Статья с важной для области идеей**

Рабочая гипотеза: важные для развития области статьи имеют высокое значение **CD (Citation Disruption)**, ориентировочно \(CD \approx 1\). Значение CD характеризует, в какой степени работа замещает предшествующие исследования в последующих цитированиях, а не просто продолжает их.

## 3. Ранжирование статей

Построено два ранжирования:

### 3.1. **По числу цитирований**
- Graph of Thoughts: Solving Elaborate Problems with Large Language Models (Besta et al., 2024). DOI: 10.1609/aaai.v38i16.29720.

- Towards Understanding Chain-of-Thought Prompting: An Empirical Study of What Matters (Wang et al., 2022). DOI: 10.48550/arXiv.2212.10001.

- SWE-RL: Advancing LLM Reasoning via Reinforcement Learning on Open Software Evolution (Wei et al., 2025). DOI: 10.48550/arXiv.2502.18449.

- An LLM Compiler for Parallel Function Calling (Kim et al., 2023). DOI: 10.48550/arXiv.2312.04511.
  
### 3.2. **По значению CD** — для выявления работ, оказавших наиболее заметное влияние на направление исследований.

#### 3.2.1 CD внутри выбранных статей

| № | Статья | Год | Internal CD | \(N_i\) | \(N_j\) | \(N_k\) |
|---:|---|---:|---:|---:|---:|---:|
| 1 | Leveraging LLM Reasoning Enhances Personalized Recommender Systems | 2024 | 1.00 | 2 | 0 | 0 |
| 2 | The Surprising Effectiveness of Negative Reinforcement in LLM Reasoning | 2025 | 1.00 | 1 | 0 | 0 |
| 3 | Efficient Reinforcement Learning with Semantic and Token Entropy for LLM Reasoning | 2025 | 1.00 | 1 | 0 | 0 |
| 4 | Sketch-of-Thought: Efficient LLM Reasoning with Adaptive Cognitive-Inspired Sketching | 2025 | 1.00 | 1 | 0 | 0 |

#### 3.2.2 Классический CD5

Ограничение: область молодая и быстроразвивающаяся

## 4. Граф цитирований

Построен граф связей между статьями в Litmaps:

[Открыть граф LLM Reasoning](https://app.litmaps.com/shared/6fc61e96-3941-4ae6-ab9c-13a4bffb7063)

## 5. Проверка результатов

### Мой выбор

### ИИ-ассистент

1. **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models** — Wei et al. (2022). Фундаментальная работа о Chain-of-Thought (CoT) prompting и генерации промежуточных шагов рассуждения. [arXiv:2201.11903](https://arxiv.org/abs/2201.11903).
2. **ReAct: Synergizing Reasoning and Acting in Language Models** — Yao et al. (2022). Подход, объединяющий рассуждение и выполнение действий, в том числе взаимодействие с внешними инструментами. [Google Research](https://research.google/blog/react-synergizing-reasoning-and-acting-in-language-models/).
3. **Tree of Thoughts: Deliberate Problem Solving with Large Language Models** — Yao et al. (2023). Исследование поиска по нескольким ветвям рассуждений с оценкой промежуточных состояний и возвратом к предыдущим шагам. [arXiv:2305.10601](https://arxiv.org/abs/2305.10601).
4. **Self-Consistency Improves Chain of Thought Reasoning in Language Models** — Wang et al. (2022). Метод повышения надёжности CoT посредством генерации нескольких цепочек рассуждений и агрегирования итоговых ответов.
5. **DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning** — DeepSeek-AI (2025). Работа о развитии способностей к рассуждению посредством обучения с подкреплением. [arXiv:2501.12948](https://arxiv.org/abs/2501.12948).

### The Periodic Table of LLM Reasoning

1. **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models** — Wei et al. Фундаментальная работа о Chain-of-Thought (CoT), показавшая эффективность пошагового рассуждения.
2. **Large Language Models are Zero-Shot Reasoners** — Kojima et al. Работа о zero-shot prompting и использовании инструкции *“Let's think step by step”* для улучшения решения задач.
3. **Self-Consistency Improves Chain of Thought Reasoning in Language Models** — Wang et al. Метод генерации нескольких цепочек рассуждений с последующим выбором наиболее согласованного ответа.
4. **Let's Verify Step by Step** — Lightman et al. Работа о процессной супервизии рассуждений и Process Reward Models (PRMs).

## Артефакты

https://colab.research.google.com/drive/1Gi68e5U8f1KH4P2TAN72IuxkHruQO95G?usp=sharing
