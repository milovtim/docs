---
sourcePath: ru/ydb/ydb-docs-core/ru/core/reference/ydb-cli/_includes/auth/env_cloud.md
---
- Если задано значение переменной окружения `IAM_TOKEN`, то используется режим аутентификации **Access Token**, в который передается значение данной переменной
- Иначе, если задано значение переменной окружения `YC_TOKEN`, то используется режим аутентификаии **Refresh Token**, а токен для передачи на IAM endpoint при перезапросе берется из значения этой переменной
- Иначе, если задано значение переменной окружения `USE_METADATA_CREDENTIALS`, равное 1, то используется режим аутентификации **Metadata**
- Иначе, если задано значение переменной окружения `SA_KEY_FILE`, то используется режим аутентификации **Service Account Key**, а ключ загружается из файла, имя которого указано в данной переменной
