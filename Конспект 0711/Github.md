# Github

## Коммит

Коммит - введение изменения

Коммиты должны быть наиболее минимальными.

При параллельной работе часто нужно будет проводить объединения. Изменения на ветке `master` проводятся через PR для более понятного слияния.

Blame позволяет посмотреть, кто последний раз трогал определённую строчку.

Коммиты стоит делать по задачам, сначала пишется индекс задачи (в системе трекинга задач), потом комментарий к задаче.

## Feature-ветки

Feature-ветки - отдельная ветка коммитов, где выполняется отдельная задача. Нужны для слияния в `master` конечного результата.

Feature-ветки должны регулярно делать `rebase` для получения новых данных с `master`, таким образом он получает изменения и конфликты постепенно.

## CI/CD

### CI

Нужны регулярные сборки, чтобы команда понимала, где находится прогресс. Но эти dev-сборки не показываются заказчику.

Каждый коммит заливает новое изменение в prod. С каждым коммитом происходит новый выпуск. С web это достаточно просто, тк пользователь постоянно обновляется.

### CD

Постепенно выпускать новую версию (1% пользователей, 2% и так далее)
