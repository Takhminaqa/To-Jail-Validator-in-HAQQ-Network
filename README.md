# To-Jail-Validator-in-HAQQ-Network
## Test of strength!
Логика действий - отправляем короткие TCP пакеты данных на p2p порт.
Чтоб узнать IP валидатора я воспользовалась поиском по пул реквестам в репозитории Github [validators-contest](https://github.com/haqq-network/validators-contest)<br/>
Затем иду на сайт [yougetsignal](https://www.yougetsignal.com/tools/open-ports/) , проверить открыт ли порт 26656.<br/>
Отправляем с помощью генератора пакетов **hping3**<br/>
Устанавливаем **hping3** командой **apt install hping3**<br/>
Команда запуска: **`hping3 -S -p 26656 -i u10 -d 1024 --flood 185.182.186.35`**<br/>
Выбираем активного валидатора,у которого виден IP адрес и открыт порт 26656  и можно начинать.<br/>
**Смотрим, что Валидатор работает и активен**<br/>
![pic1](https://github.com/Takhminaqa/To-Jail-Validator-in-HAQQ-Network/blob/main/asset/1pic.png)
