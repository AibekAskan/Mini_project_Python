# Мини-проект Python: Обработка данных пользователей

Этот проект предназначен для работы с файлом `users.txt`, содержащим данные о пользователях. В рамках проекта выполняются следующие задачи:

## Функциональность

1. **Чтение файла `users.txt`**
   - Программа читает файл построчно.
   - Используется обработка исключений `try-except`:
     - Если файл не найден, выводится сообщение: *"the file that you would like to read is not found"*.
     - Для любых других ошибок выводится сообщение: *"some error occurred"*.

2. **Класс `Users`**
   - Атрибуты:
     - `first_name` (Имя)
     - `last_name` (Фамилия)
     - `birth_year` (Год рождения)
     - `email` (Адрес электронной почты)
   - Метод:
     - `getAge()`: вычисляет возраст пользователя на основе текущего года (2023).

3. **Создание списка пользователей**
   - Каждая строка файла преобразуется в объект класса `Users`.
   - Данные разделяются с помощью `split(',')`.
   - Все объекты сохраняются в список пользователей.

4. **Фильтрация пользователей**
   - Функция `filter_users(low=30, high=50, users=[])`:
     - Принимает список пользователей и фильтрует их по возрасту.
     - Возвращает только тех, чей возраст больше `low` и меньше `high`.
     - Выводит отфильтрованные данные в формате: `email, возраст`.

## Как использовать

1. Убедитесь, что у вас есть файл `users.txt` с данными пользователей в формате:
   ```
   Имя,Фамилия,ГодРождения,Email
   John,Doe,1990,johndoe@example.com
   Jane,Smith,1985,janesmith@example.com
   ```
2. Запустите программу.
3. Проверьте, что в консоли выводятся:
   - Ошибки (если есть проблемы с файлом)
   - Список отфильтрованных пользователей по возрасту.

## Требования
- Python 3+
- Файл `users.txt` в корневой папке проекта

## Авторы
Разработано в рамках учебного проекта по Data Analytics.

