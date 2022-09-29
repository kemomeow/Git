# Git-
Nmap («Network Mapper») - это утилита с открытым исходным кодом для исследования сети и проверки безопасности. Она была разработана для быстрого сканирования больших сетей, хотя прекрасно справляется и с единичными целями. Nmap использует "сырые" IP пакеты оригинальным способом, чтобы определить какие хосты доступны в сети, какие службы (название приложения и версию) они предлагают, какие операционные системы (и версии ОС) они используют, какие типы пакетных фильтров/брандмауэров используются и еще множество других характеристик. В то время, как Nmap обычно используется для проверки безопасности, многие системные администраторы находят ее полезной для обычных задач, таких как контролирование структуры сети, управление расписаниями запуска служб и учет времени работы хоста или службы.
Выходные данные Nmap это список просканированных целей с дополнительной информацией по каждой из них в зависимости от заданных опций. Ключевой информацией является «таблица важных портов». Эта таблица содержит номер порта, протокол, имя службы и состояние. Состояние может иметь значение open (открыт), filtered (фильтруется), closed (закрыт) или unfiltered (не фильтруется). Открыт означает, что приложение на целевой машине готово для установки соединения/принятия пакетов на этот порт. Фильтруется означает, что брандмауэр, сетевой фильтр, или какая-то другая помеха в сети блокирует порт, и Nmap не может установить открыт этот порт или закрыт. Закрытые порты не связаны ни с каким приложением, но могут быть открыты в любой момент. Порты расцениваются как не фильтрованные, когда они отвечают на запросы Nmap, но Nmap не может определить открыты они или закрыты. Nmap выдает комбинации открыт|фильтруется и закрыт|фильтруется, когда не может определить, какое из этих двух состояний описывает порт. Эта таблица также может предоставлять детали о версии программного обеспечения, если это было запрошено. Когда осуществляется сканирование по IP протоколу (-sO), Nmap предоставляет информацию о поддерживаемых протоколах, а не об открытых портах.
Типичный пример сканирования с помощью Nmap
# nmap 

Starting Nmap ( https://nmap.org )
Interesting ports on scanme.nmap.org (64.13.134.52):
(The 1663 ports scanned but not shown below are in state: filtered)
PORT    STATE  SERVICE VERSION
22/tcp  open   ssh     OpenSSH 3.9p1 (protocol 1.99)
53/tcp  open   domain
70/tcp  closed gopher
80/tcp  open   http    Apache httpd 2.0.52 ((Fedora))
113/tcp closed auth
Device type: general purpose
Running: Linux 2.4.X|2.5.X|2.6.X
OS details: Linux 2.4.7 - 2.6.11, Linux 2.6.0 - 2.6.11

Interesting ports on playground.nmap.org (192.168.0.40):
(The 1659 ports scanned but not shown below are in state: closed)
PORT     STATE SERVICE       VERSION
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn
389/tcp  open  ldap?
445/tcp  open  microsoft-ds  Microsoft Windows XP microsoft-ds
1002/tcp open  windows-icfw?
1025/tcp open  msrpc         Microsoft Windows RPC
1720/tcp open  H.323/Q.931   CompTek AquaGateKeeper
5800/tcp open  vnc-http      RealVNC 4.0 (Resolution 400x250; VNC port: 5900)
5900/tcp open  vnc           VNC (protocol 3.8)
MAC Address: 00:A0:CC:63:85:4B (Lite-on Communications)
Device type: general purpose
Running: Microsoft Windows NT/2K/XP
OS details: Microsoft Windows XP Pro RC1+ through final release
Service Info: OSs: Windows, Windows XP

Nmap finished: 2 IP addresses (2 hosts up) scanned in 88.392 seconds
**1.** Скачал приложение![image](https://user-images.githubusercontent.com/112854659/193035518-b3125d6d-ad39-46d1-b574-9f159bf65f18.png)

**2.** Открыл приложение ![image](https://user-images.githubusercontent.com/112854659/193036116-5cc87bd1-56c5-4ee4-ab8f-380ff2bfb807.png)

**3.** Ввел цель![image](https://user-images.githubusercontent.com/112854659/193036387-fb953de5-6702-4d07-93d7-c7e22e250c8e.png)

**4.** Выбрал интенсивное сканирование ![image](https://user-images.githubusercontent.com/112854659/193036798-da622154-1c42-4e6f-b0b0-888f6a84080c.png)

**5.** Просканировал сеть интернет ![image](https://user-images.githubusercontent.com/112854659/193037156-d44414b8-8423-43aa-bba2-2eb84775f785.png)
![image](https://user-images.githubusercontent.com/112854659/193037277-8f3ddaaf-8baa-462c-9f61-66ad205260ca.png)
![image](https://user-images.githubusercontent.com/112854659/193037328-45d21c55-f9d9-4488-b65d-590fea62b4d4.png)
![image](https://user-images.githubusercontent.com/112854659/193037380-55e8f5da-bf6c-4939-b234-9268edf58912.png)
![image](https://user-images.githubusercontent.com/112854659/193037457-c82ff886-fbf1-4749-9933-1cde66c62ce0.png)



