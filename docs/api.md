# API Спецификация (v1.0.2)

Все запросы к API должны содержать заголовок `Authorization: Bearer <token>`.

| Метод | Эндпоинт | Описание |
|-------|----------|----------|
| GET | `/api/v1/kb/articles` | Получить список всех статей БЗ |
| POST | `/api/v1/tests/generate` | Создать задачу на генерацию теста ИИ |
| GET | `/api/v1/user/stats` | Получить статистику прогресса |
| PATCH | `/api/v1/moderation/report` | Отправить жалобу на контент |

### Пример запроса на генерацию теста:
```json
{
  "document_id": "uuid-12345",
  "difficulty": "medium",
  "question_count": 15,
  "language": "ru"
}