&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***Форма ввода данных о возрасте сервиса получения паспорта***   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***гражданина Российской Федерации***

|**Группа проверок**|**Название класса**|**Границы**|**Тестовые данные внутри класса (содержимое поля)**|**Тестовые данные на границах (содержимое поля)**|**Системное сообщение**|
|:------:|:--------------:|:--------------:|:---------------:|:-------------:|:--------:|
| `Возраст гражданина` | возраст от 0 до 14 лет | [0, 13] | 7 | 0, 1, 12, 13, ~~14~~ | "Нельзя оформить" |
| `Возраст гражданина` | возраст от 14 до 116 лет | [14, 115] | 65 | ~~13~~, 14, 15, 114, 115, ~~116~~ | "Можно оформить" |
| `Возраст гражданина` | возраст от 116 лет | [116] | 300 | 116 | "Ошибка" |
