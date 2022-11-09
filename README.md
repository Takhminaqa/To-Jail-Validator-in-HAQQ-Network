# To-Jail-Validator-in-HAQQ-Network
## Test of strength!
Ru. Логика действий - отправляем короткие TCP пакеты данных на p2p порт.
Чтоб узнать IP валидатора я воспользовалась поиском по пул реквестам в репозитории Github [validators-contest](https://github.com/haqq-network/validators-contest)<br/>
En. Action logic - we send short TCP data packets to the p2p port.
To find out the IP of the validator, I used the pull request search in the Github repository [validators-contest](https://github.com/haqq-network/validators-contest)<br/>


Ru. Затем иду на сайт [yougetsignal](https://www.yougetsignal.com/tools/open-ports/) , проверить открыт ли порт 26656.<br/>
Отправляем с помощью генератора пакетов **hping3**<br/>
Устанавливаем **hping3** командой **apt install hping3**<br/>
Команда запуска: **`hping3 -S -p 26656 -i u10 -d 1024 --flood 185.182.186.35`**<br/>
Выбираем активного валидатора,у которого виден IP адрес и открыт порт 26656  и можно начинать.<br/>
En. Then I go to the site [yougetsignal](https://www.yougetsignal.com/tools/open-ports/) , check if port 26656 is open.<br/>
Sending using the packet generator **hping3**<br/>
Install **hping3** with **apt install hping3**<br/>
Run command: **`hping3 -S -p 26656 -i u10 -d 1024 --flood 185.182.186.35`**<br/>
Select an active validator that has an IP address visible and port 26656 open, and you can start.<br/>**Смотрим, что Валидатор работает и активен**<br/>
![pic1](https://github.com/Takhminaqa/To-Jail-Validator-in-HAQQ-Network/blob/main/asset/1pic.png)

Запускаем команду, и видим, через несколько минут Валидатор начинает пропускать. 
We run the command, and we see that after a few minutes the Validator starts to skip.<br/>
![pic2](https://github.com/Takhminaqa/To-Jail-Validator-in-HAQQ-Network/blob/main/asset/2pics.png)

Прерываем команду 3 раза. 
We interrupt the command 3 times.![pic3](https://github.com/Takhminaqa/To-Jail-Validator-in-HAQQ-Network/blob/main/asset/3pics.png)
![pic4](https://github.com/Takhminaqa/To-Jail-Validator-in-HAQQ-Network/blob/main/asset/4pics.png)
![pic5](https://github.com/Takhminaqa/To-Jail-Validator-in-HAQQ-Network/blob/main/asset/5pics.png)

RU. Подытожим интересное задание. Если не прерывать команду, через несколько минут Валидатор начинает пропускать блоки и в итоге оказывается в тюрьме. По скринам понятно, что пропуск блоков был инициирован мной т.е извне.<br/>
En. To sum up this  interesting task. If you don't interrupt the team, after a few minutes the Validator starts skipping blocks and ends up in jail. From the screenshots, it is clear that the skipping of blocks was initiated by me, i.e. from the outside.
