# В команде только 1 участник: Айдунбеков Кунах. Причина поздно приступил к решению задания. А также примерно 15.03.2023 сбросилась авторизация из Slack. 
# После неудачной попытки авторизоваться повторно, забросил эту идею. Так как общели новую программу бля связи, но ссылку я там и не получил на e-mail.
# А также разочарование самой платформой. Куча разных чатов, которые живут своей жизнью, и на вопрос получаешь стандартный ответ переадресации в другой чат и тд. 
# ИМХО: Флудилка в телеге была бы куда полезней, + возможность нормального общения с сокурсниками

# Описание идею проста: мини мессенджер с сохранением истории общения

# Описание пользовательских типов и функций приведено в коде комментариями, а также попыткой написать читабельный код - Очень жду развернутой оценки стиля написания кода, не хочу спагети писать 
# Роли не были распределены, так как писал код один, в течении 3 мартовских вечеров

# ConsoleMessenger - Консольная программа для обмена сообщениями
# В данной программе реализована вожность отправки сообщений в общий чат и приватные чаты
# Общий чат доступен для всех пользователей зарегистрироващихся в программе
# Доступ к приватному могут получить только 2 пользователя по ID чата. 
# При желании пользователь может создать приватный чат с каждым из других пользователей системы. При этом есть обработка повторной попытки создать чат с одним и тем же пользователем.
# Информация о зарегестрированных пользователях и переписке в чатах хранится в txt файлах. Сделано для удобства, чтобы не производить повторный ввод данных при перезапуске программы.
# Для удобства пользования реализованы консольные интерфейсы с инструкциями. А также обработка ввода данных пользователем, чтобы исключить непредвиденные ситуации ввода данных.
# Запись и чтение файлов таже осуществляются с проверкой. Было принятно решение не использовать конструкицю try cath, так как нет ситуации когда один файл читается несколькими пользователями.
# Также не использовалиль шаблонные функции/классы, из-за однатипности данных.
# Реализовано публичное и защищенное наследование классов
# Файлы txt делятся на 2 типа: 1-ый хранит историю переписки чата, где каждая строка это отдельное сообщение, сами сообщение логируются именем отправителя и временем отправки;
# 2-ой тип файлов хранит структуру данных пользоватлеся: name	login	password, и данных об приватных чатах пользователя: chatID		loginCompanion.
# Для оптимизации работы программы, подгрузка данных приватных чатов производится только в случае если пользователь зашел в раздел "личные чаты"
# Еще одним преимуществом данной программы, является возможность: регистрации, авторизации и выхода/входа из учетной записи во время работы программы без ее перезапуска.
# На этом я устал, так как полтора часа возился с загрузкой в репозиторий из-за проблем с папкой .vs ("Слишком тяженый мусор от VS2022")

# P.S. 29.03.2023 23:46:52  - Успел до 30.03.2023 )