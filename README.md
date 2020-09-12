[build]:  https://travis-ci.org/github/abramov1982/E1.12

[Result:] https://travis-ci.org/abramov1982/E1.12.svg?branch=master

  Запуск игры:
  - python hangman.py

  Запуск теста для pytest:
  - coverage run -m --source=. pytest tests/test_pytest.py
  - coverage report -m

Или файлы  hangman.py и test_pytest.py из PyCharm

Текст в консоли должен выводится с цветными вставками.
На Linux обязательно, на Win, если подключены Ascii коды.
В Win нужно убрать в программе Hangman.py
комментарии (#) перед
# import colorama
# colorama.init()
иначе в командной строке будут видны служебные символы оператора print()!!!
Хочу уточнить, что модуль colorama не загружается в Travis CI
там этот модуль выдает ошибку.
Именно по этому, эти два операнда закоментированны в варианте размещенном на GitHub.
По совету юнита 11 в E1 - статус последней сборки добавлен в README.md.
