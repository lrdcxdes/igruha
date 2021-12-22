Простой пример использования библиотеки:

* Устанавливаем библиотеку
```commandline
python -m pip install igruha
```

* Пример кода
```python
from igruha import Igruha

parser = Igruha()
games = parser.search('Far Cry').games

for game in games:
    game.get_details()
    print('Игра: %s\nТрейлер: %s' % (game.name, game.trailer) )

games[0].download('Custom name') #Скачать игру
```

Дополнительная информация и методы: https://github.com/LORD-ME-CODE/igruha