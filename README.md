# Firebase
Working with databases Firebase.

Чтобы сгенерировать файл закрытого ключа для вашей учётной записи службы:

1) В Firebase консоли откройте *Настройки > [Учётные записи служб](https://console.firebase.google.com/project/_/settings/serviceaccounts/adminsdk)*.

2) Нажмите кнопку *Создать новый секретный ключ*, а затем подтвердить, нажав *Создать ключ*.

3) Надёжно храните файл JSON, содержащий ключ.



## Cloud Firestore

Более полное руководство здесь: [Начать работу с Cloud Firestore](https://firebase.google.com/docs/firestore/quickstart)



## Realtime Database

Более полное руководство здесь: [Начать работу с Realtime Database](https://firebase.google.com/docs/database/admin/start)

Для базы укажите следующие разрешения:

<code>
{ 
  "rules": { 
    "books" : { 
          ".indexOn": ["Price", "Author", "Genre", "Title", "value"] 
        }, 
    ".read": true, 
    ".write": true, 
  } 
} 
</code>



## Параметры

Для работы с ноутбуком впишите следующие параметры подключения:

SERVICE_ACCOUNT_KEY - Имя файла закрытого ключа.

DATABASE_NAME - Имя базы данных.

DATABASE_SERVER - Сервер базы данных.

