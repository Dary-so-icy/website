# website
# сайт для поиска занятий
**Инструкция по применению**
Скачать все файлы как архив; распаковать архив.
С помощью файла requirements.txt установить зависимые библиотеки.
Запустить файл main.py 


**Модели проекта**
модель user: пользователь(ученик или учитель). есть поля role (ученик или учитель) ,surname(фамилия), name(имя),  age(возраст), phone(телефон, тип integer, вводить начиная с 8 , а не с +7), emai(почта) , about_me(о человеке, мини резюме), hashed_password(пароль)

модель subject: модель для предметов. поля:  name(название предмета ), about(немного о предмете, например : физика для 10 классов для выравнивания знаний по предмету ),   is_hard( поле типа boolean, обозначает сложныЙ ли уровень предмета, True- сложный, False- нет, по умолчанию False),  user(связь с таблицей учителей которые ведут этот предмет)

Модель lesson: поля:   name(название занятия с репетитором), time( на какое время назначено занятие ),   place(место где будет занятие( я хочу если получится попытаться выводить его на карту Яндекс было бы круто)),  about( немного о занятии, сюда учитель может написать например дз). Есть связь с другой моделью через параметр subject

