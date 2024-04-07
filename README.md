# VIDA на MacOS

## Установка UTM

- ставимо пакетний менеджер `brew` - за його допомогою будемо інсталювати UTM і всі необхідні залежності

Відкриваємо Terminal і виконуємо команду:

```
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
 ```

- ставимо Xcode 

```
 xcode-select --install
``` 

- нарешті, запускаємо установку UTM

```
brew install utm
```

- ставимо додаткові пакети для роботи UTM

```
brew install qemu
brew install aria2

brew tap sidneys/homebrew
brew install cabextract wimlib cdrtools

brew tap minacle/chntpw
brew install minacle/chntpw/chntpw

```

## Створення віртуальної машини з готового образу VIDA

- Завантажуємо [образ](https://www.dropbox.com/scl/fi/jgsean0efih2ba5t73czu/VIDA_ru.zip?rlkey=aj6fu2y7efomp3hd8syey3ws9&dl=0) віртуальної машини з уже встановленою та налаштованою VIDA

- Розпаковуємо архів, відкриваємо UTM, створюємо нову віртуальну машину

![створення нової вм](img/utm_create_vm.png)

- На наступному кроці обираємо відкрити існуючий образ і вказуємо шлях до раніше розпакованого файлу

![відкриваємо образ](img/utm_open_vm.png)

![вказуємо шлях до файлу](img/utm_load_image.png)

![віртуальна машина створена](img/utm_vm_created.png)

- Запускаємо віртуальну машину

![запуск віртуальної машини](img/utm_start_vm.png)

- Чекаємо поки стартує сервіс VIDA

![VIDA запущено](img/utm_vida_started.png)

- Відкриваємо VIDA, вводимо логін (наприклад, 4) - PROFIT!

![VIDA вхід](img/utm_vida_login.png)

- Додаємо профіль свого авто і можна користуватись

![VIDA профіль авто](img/utm_vida_car_add.png)
