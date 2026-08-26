## 🚀 Postman API Testing — Swagger Petstore (CRUD & Request Chaining)

Автоматизований тестовий набір у Postman для перевірки REST API сервісу Swagger Petstore. Проєкт демонструє побудову повного CRUD-циклу, генерацію динамічних тестових даних та зв'язування запитів.

### 📌 Ключові особливості та реалізований функціонал:
* **CRUD Cycle Coverage:** Реалізовано повний цикл операцій (`POST`, `GET`, `PUT`, `DELETE`) для сутності `Pet`.
* **Pre-request Scripts:** Автоматична генерація унікальних тестових даних (`petId`, `petName`) перед відправкою запиту (`Math.random()`) для запобігання дублюванню даних у БД.
* **Request Chaining:** Передача динамічного `petId` між запитами за допомогою глобальних змінних Postman (`pm.globals.set` / `{{petId}}`).
* **Post-response Assertions:** Автоматичні перевірки (Status Codes 200/404, перевірка структури та значень полів у JSON-відповіді).
* **Negative Testing:** Перевірка обробки помилок сервером (статус `404 Not Found` після видалення об'єкта).
* **Automated Execution:** Повний запуск усієї тестової сюїти в один клік через **Collection Runner**.

---

### 🛠 Структура тестового сценарію (Test Suite Workflow)

1. `POST /pet` — Створення нової тваринки з динамічним `petId` та `petName` (**Before request script** + перевірка status code 200 та імені у відповіді).
2. `GET /pet/{petId}` — Отримання даних створеної тваринки за допомогою **Request Chaining** (`{{petId}}`).
3. `PUT /pet` — Оновлення імені на `"Barsik Super"` та статусу на `"sold"` (перевірка збігу оновлених полів у JSON).
4. `DELETE /pet/{petId}` — Видалення об'єкта за `{{petId}}` (перевірка успішного статусу 200).
5. `GET /pet/{petId}` — Перевірка негативного сценарію (підтвердження видалення об'єкта зі статусом `404 Not Found`).

---

### 📁 Як запустити колекцію локально:

1. Завантажте файл [Petstore CRUD Tests.postman_collection.json](./Petstore%20CRUD%20Tests.postman_collection.json) з цього репозиторію.
2. Відкрийте **Postman** та натисніть кнопку **Import** (у лівому верхньому кутку).
3. Оберіть завантажений `.json` файл.
4. Клацніть на **`...`** біля назви колекції `Petstore CRUD Tests` ➔ виберіть **Run collection**.
5. Натисніть **Run Petstore CRUD Tests** для автоматичного запуску всіх тестів.
