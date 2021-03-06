Поток событий 
# Оглавление 

# 1. Актеры 
| Актер | Пользователь|
|:-----:|:----------- |
| Пользователь, которому отображаются какие-то задачи | Пользователь, у которого на запускаемом компьютере в локальном хранилище имеются данные для приложения |
| Пользователь, у которого все списки пустые | Пользователь, у которого на запускаемом компьтере в локальном хранилище не имеются данные для приложения |

# 2. Варианты использования
## 2.1 Добавление задачи
*Описание:* Вариант использования "Добавление задачи" позволяет добавлять задачу в приложение. 
*Предусловие:* Пользователь ввел информацию о задаче в поле ввода.
*Основной поток* 
1. Заметить нажатие кнопки
2. Проверить введен ли дедлайн задачи. Если нет, то далее выполняется альтернативный поток А1. 
3. Сохранить задачу с полученными данными в локальное хранилище.
4. Сохранить задачу в локальном хранилище 
5. Если на главном экране отображается категория задач, которая удовлетворяет добавленной задаче - отобразить данную задачу в список находящийся на главном экране.
*Альтернативный поток А1*
1. Уточнить у пользователя пустое поле даты дедлайна. 
2. При подтверждении пустой даты дедлайна - перейти к п. 3 основного потока.
3. Показать пользователю всплывающиее окно с полем для ввода даты дедлайна. 
4. Перейти к п.3 основоного потока.
## 2.2 Просмотр задач по категориям 
*Описание:* Вариант использования "Просмотр задач по категориям" позволяет просматривать имеющиеся задачи по категориям.
*Основной поток*
1. Заметить нажатие по любому из предложенных списков.
2. Просмотреть все задачи хранящиеся в локальном хранилище.
3. Выбрать те из них, которые удовлетворяют выбранному списку. 
4. Отобразить выбранные задачи на главном экране. Если список задач оказался пустым, то будет отображен специальный вариант /*вставить ссылку на пустой мокап*/ главного экрана. 
## 2.3 Поиск задач по ключевым словам
*Описание:* Вариант использования "Поиск задач по ключевым словам" позволяет найти все задачи по введенным ключевым словам. 
*Основной поток*
1. Заметить нажатие по кнопке "Search".
2. Если поле ввода ключевых слов является пустым, то далее выполняется альтернативный поток А1.
3. Данные введенные в поле ввода ключевых слов считать ключевыми словами. Чтобы дальнешие изменения данного поля во время выполнения варианта использования не повлияли на результат отображенный на экране.  
4. Просмотреть все задачи хранящиеся в локальном хранилище.
5. Выбрать те из них, которые удовлетворяют ключевым словам. 
6. Отобразить выбранные задачи на главном экране. Если список задач оказался пустым, то будет отображен специальный вариант /*вставить ссылку на пустой мокап*/ главного экрана. 
*Альтернативный поток А1*
1. Показать пользователю всплывающее окно, которое сообщает, что ключевых слов для поиска введено не было. 
2. Уточнить у пользователя пустое поле ключевых слов. 
3. При подтверждении пустого поля ввода ключевых слов - показать пользователю пустое главное окно. Иначе перейти к альтернативному потоку А2. 
*Альтернативный поток А2*
1. Показать пользователю всплывающее окно с формой для ввода ключевый слов. 
2. Заметить нажатие по кнопке "Search". 
3. Если поле ввода ключевых слов оказалось пустым, то перейти к альтернативному потоку А1. Иначе введенную информацию считать ключевыми словами и перейти к п. 4 основного потока. 
## 2.4 Удаление задачи
*Описание:* Вариант использования "Удаление задачи" позволяет удалять задачи без сохранения любой информации о них.
*Предусловие:* До начала работы варианта использования "Удаление задачи" должна отображаться хотя бы одна активная задача. 
*Основной поток*
1. Заметить нажатие по крестику возле любой из задач. 
2. Определить какой задаче соответсвуюет данный крестик. 
3. Удалить данную задачу из локального хранилища. 
4. Обновить отображение главного экрана. Если список отображения оказался пустым, то показать пустой /*вставить ссылку*/вариант главного экрана.
## 2.5 Отметка задачи как выполненной 
*Описание:* Вариант использования "Отметка задачи как выполненной" позволяет отмечать задачи как выполненные. 
*Предусловие:* До начала работы варианта использования "отметка задачи как выполненной" должна отображаться хотя бы одна активная задача. 
*Основной поток*
1. Заметить нажатие по чекбоксу возле любой из задач. 
2. Определить какой задаче соответсвуюет данный чекбокс. 
3. Удалить данную задачу из локального хранилища. 
4. Обновить отображение главного экрана. Если список отображения оказался пустым, то показать пустой /*вставить ссылку*/вариант главного экрана.