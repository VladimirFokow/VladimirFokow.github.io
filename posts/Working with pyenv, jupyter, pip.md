---
label: Working with pyenv, pip, Jupyter (on MacOs)
---

# Working with pyenv, pip, Jupyter

Here I will share my personal notes which I find very useful when working with pyenv, pip, and Jupyter on MacOS.


*Note: this post is a work in progress*

---

**Managing Multiple Python Versions With pyenv:**

https://realpython.com/intro-to-pyenv/


---

Посмотреть доступные версии python для установки (отфильтрованные grep-ом)
pyenv install --list | grep " 3\.[678]"
pyenv install -l | grep '^  3.10'

Посмотреть установленные версии python
pyenv versions

Установить версию python
pyenv install <version>

Удалить версию python
    !!!Но версия может ведь быть необходима для какого-то виртуального окружения!!!
    !!!Нельзя удалять системную версию - она нужна компьютеру!!!
    (виртуальное окружение удаляется так же)
pyenv uninstall 3.7.0


Если написать [version-number], то эта версия установится, иначе просто покажется текущая установленная
    (можно несколько версий, но как только первая находится, остальные будут проигнорены)
pyenv global [version-number]       - глобальная
pyenv local [version-number]        - в конкретной папке, где произведена команда
(ещё есть уровень shell)


---

*to be continued...*