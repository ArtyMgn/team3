Контроллер распологается по относительному адресу `/api`

Методы 
- GET `/chats` возвращает список чатов и последнее сообщение в этом чате для залогиненного 
пользователя
- GET `/chats/{id}/messages` возвращает список сообщений для чата с id=id
- GET `/users/{id}` возвращает объект пользователя с id=id
- POST `/chats` создает чат, в body необходимо передать { title: '...', interlocutorId: '...' }
- POST `/users` создает пользавателя при первом логине, в теле фапроса необходимо послать объект,
 который вернулся с при логине на гитхабе
- POST `/chats/{id}/messages` добавляет сообщение в чат с id=id