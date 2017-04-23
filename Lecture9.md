# Лекция девятая
Все слайды [тут](http://melevir.com/static/styleru_py/slides/9.html).

### Логирование

[Слайд 4](http://melevir.com/static/styleru_py/slides/9.html?full#4)
- Форматировать сообщения проще, потому что формат достаточно задать в одном месте и переиспользовать везде.
- Если `print` приходится удалять, то какие-нибудь `logger.debug` никому не мешают в коде потому что мы можем регулировать уровень отобажаемых сообщений.
- У нам не всегда доступна консоль, поэтому бывает удобно записывать логи куда-то еще. Например, во внешний сервис, который будет присылать письма об ошибках.

[Слайды 9-10](http://melevir.com/static/styleru_py/slides/9.html?full#9):
- В продакшене часто используют только уровни `DEBUG` и `ERROR`.

### Окружение приложения

[Слайд 11](http://melevir.com/static/styleru_py/slides/9.html?full#11):
- Да-да, сервер — это обычный компьютер. Вау.

[Слайд 14](http://melevir.com/static/styleru_py/slides/9.html?full#14):
- Реальный компьютер можно разбить на несколько виртуальных. Так и делают облачные провайдеры.

[Слайды 20-22](http://melevir.com/static/styleru_py/slides/9.html?full#20):
- С приложением и веб-сервером разобрались, осталось понять, что такое wsgi-интерфейс.

### Развертывание и деплой
[Слайды 29-30](http://melevir.com/static/styleru_py/slides/9.html?full#29):
- Помимо перечисленного, для развертывания кода нужно сделать куда больше. 

[Слайды 35-36](http://melevir.com/static/styleru_py/slides/9.html?full#35):
- Фабрик позволяет написать небольшой скрипт на Питоне, который проведет развертывание за вас.

### CI

[Слайд 39](http://melevir.com/static/styleru_py/slides/9.html?full#39):
- Например, получаете вы пулл реквест. Можно, конечно, попытаться развернуть и протестировать его на своей машине, а можно настроить CI, который будет это делать за вас и говорить, работает ли код в пулл реквесте. 
- Если код в мастере все-таки сломается, CI пришлет об этом письмо и в целом сделает это заметнее.

[Слайд 40](http://melevir.com/static/styleru_py/slides/9.html?full#40):
- Jenkins и Travis — два самых популярных сервиса для CI. Jenkins дольше настраивать, но у него открытый исходный код. 
- С другой стороны, Travis бесплатный для проектов с открытым исходным кодом.

### Слепая десятипальцевая печать

[Слайд 42](http://melevir.com/static/styleru_py/slides/9.html?full#42):

- Слепая десятипальцевая печать помогает думать над чем, что печатаешь, и не задумываться, как это печатать. И экономит это очень много времени.
- Опечатки веб-разработчику тоже стоят время.
- Научиться нормально печатать можно, например, на nabiraem.ru. 