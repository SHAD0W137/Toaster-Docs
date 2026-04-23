
# Руководство разработчика

<a id="arch"></a>
### Архитектура системы
Система ToasterEX построена на микросервисной архитектуре:
* **Frontend**: React Native (Web/Mobile).
* **Backend**: Flask (Python 3.11).
* **AI Service**: Интеграция с OpenAI API / Anthropic через прокси-слой.
* **Cache**: Redis для хранения сессий тестирования.

<a id="git"></a>
### Git Workflow
Мы придерживаемся стратегии **Feature Branching**:
1. `main` — только стабильные релизы.
2. `develop` — интеграционная ветка.
3. Каждая новая задача делается в ветке `feature/task-name`.

**Стандарт коммитов (Conventional Commits):**
* `feat:` — новая функциональность.
* `fix:` — исправление багов.
* `docs:` — обновление документации (как сейчас).