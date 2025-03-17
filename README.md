# Домашнее задание к занятию "`Уязвимости и атаки на информационные системы`" - `Татаринцев Алексей`



---

### Задание 1
```
Скачайте и установите виртуальную машину Metasploitable: https://sourceforge.net/projects/metasploitable/.

Это типовая ОС для экспериментов в области информационной безопасности, с которой следует начать при анализе уязвимостей.

Просканируйте эту виртуальную машину, используя nmap.

Попробуйте найти уязвимости, которым подвержена эта виртуальная машина.

Сами уязвимости можно поискать на сайте https://www.exploit-db.com/.

Для этого нужно в поиске ввести название сетевой службы, обнаруженной на атакуемой машине, и выбрать подходящие по версии уязвимости.

Ответьте на следующие вопросы:

Какие сетевые службы в ней разрешены?
Какие уязвимости были вами обнаружены? (список со ссылками: достаточно трёх уязвимостей)
Приведите ответ в свободной форме.
```
1. `Скачиваю дистрибутив Kali  и ВМ для тренировки  Metasploitable`
2. `Настраиваю сеть и проверяю что Kali (192.168.1.5) пингует машину Metasploitable (192.168.1.10)`

![15](https://github.com/Foxbeerxxx/inf_sec1/blob/main/img/img15.png)`

3. `Сканируем в офлайн режиме Meta `
```
nmap -sV 192.168.1.10
```
![1](https://github.com/Foxbeerxxx/inf_sec1/blob/main/img/img1.png)`

4. `Видим результат открых портом  и версию сервиса`
```
 Какие уязвимости были вами обнаружены?
    *   vsftpd 2.3.4 Backdoor Command Execution: (https://www.exploit-db.com/exploits/17491) - Эта версия vsftpd *специально* содержит бэкдор, позволяющий удаленно выполнять команды.  Достаточно подключиться к FTP серверу и использовать команду USER <user>: и PASS <password>

    *   UnrealIRCd 3.2.8.1 - Backdoor Command Execution: [https://www.exploit-db.com/exploits/32702](https://www.exploit-db.com/exploits/32702) - UnrealIRCd версии 3.2.8.1 содержит бэкдор, который позволяет злоумышленнику удаленно выполнять команды на сервере. Metasploitable как раз использует уязвимую версию.

```

---

### Задание 2
```
Проведите сканирование Metasploitable в режимах SYN, FIN, Xmas, UDP.

Запишите сеансы сканирования в Wireshark.

Ответьте на следующие вопросы:

Чем отличаются эти режимы сканирования с точки зрения сетевого трафика?
Как отвечает сервер?
```

1. `Запрос SIN`

```
nmap -sS 192.168.1.10
```
![2](https://github.com/Foxbeerxxx/inf_sec1/blob/main/img/img2.png)`


2. `Заполните здесь этапы выполнения, если требуется ....`
3. `Заполните здесь этапы выполнения, если требуется ....`
4. `Заполните здесь этапы выполнения, если требуется ....`
5. `Заполните здесь этапы выполнения, если требуется ....`
6. 

```
Поле для вставки кода...
....
....
....
....
```

`При необходимости прикрепитe сюда скриншоты
![Название скриншота 2](ссылка на скриншот 2)`


---

### Задание 3

`Приведите ответ в свободной форме........`

1. `Заполните здесь этапы выполнения, если требуется ....`
2. `Заполните здесь этапы выполнения, если требуется ....`
3. `Заполните здесь этапы выполнения, если требуется ....`
4. `Заполните здесь этапы выполнения, если требуется ....`
5. `Заполните здесь этапы выполнения, если требуется ....`
6. 

```
Поле для вставки кода...
....
....
....
....
```

`При необходимости прикрепитe сюда скриншоты
![Название скриншота](ссылка на скриншот)`

### Задание 4

`Приведите ответ в свободной форме........`

1. `Заполните здесь этапы выполнения, если требуется ....`
2. `Заполните здесь этапы выполнения, если требуется ....`
3. `Заполните здесь этапы выполнения, если требуется ....`
4. `Заполните здесь этапы выполнения, если требуется ....`
5. `Заполните здесь этапы выполнения, если требуется ....`
6. 

```
Поле для вставки кода...
....
....
....
....
```

`При необходимости прикрепитe сюда скриншоты
![Название скриншота](ссылка на скриншот)`
