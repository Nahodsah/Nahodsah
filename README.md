# [Александр Находкин] | ML Researcher

**Москва | [nepershina107@gmail.com] | [@SashaNakhodkin]**

---

### Научные интересы

Математическое моделирование предиктивных систем • Машинное обучение с низкой латентностью • Оптимизация алгоритмической производительности • Промышленное тестирование моделей

---

### Технические навыки

**Языки:** Python (PyTorch, NumPy), C++ (STL, performance-critical code)  
**ML инжиниринг:** Квантизация, A/B тестирование, regression validation, оптимизация latency  
**Математика:** Теория оптимизации, стохастические процессы, линейная алгебра, численные методы  
**Системы:** Linux, Docker, Git, CI/CD basics

---

### Проекты

#### 1. Классификация персонажей Симпсонов: Production-Grade оптимизация CNN
Соревнование в формате Kaggle с реализацией кастомной CNN с нуля.

**Ключевые метрики:**  
- 94.3% top-1 accuracy, 0.89 F1-score (private leaderboard)  
- 12ms средняя latency инференса (batch=1, CPU)  
- Размер модели: 2.1MB

**Техническая реализация:**  
- Кастомная 6-слойная CNN со сжатой архитектурой для скорости  
- Ручной gradient clipping и кастомный LR scheduler (cosine annealing)  
- Data pipeline: 4-thread prefetching, RAM caching для устранения IO  
- **Код:** `src/simpsons_cnn/` | **Лог валидации:** `reports/metrics_validation.log`
