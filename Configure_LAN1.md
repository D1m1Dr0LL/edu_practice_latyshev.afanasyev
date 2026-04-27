# Часть 1

## Шаг 1. Построить сеть с топологией

<img width="2448" height="881" alt="image" src="https://github.com/user-attachments/assets/3f81aa5c-7da1-4a3c-8e6d-34934fc65992" />

*Нужно зайти в командную строку (CLI)  и включить порты на устройствах с красными индикаторами(R1, R2, R3), те же команды для другой стороны только вместо Fa0/0 меняем на Fa0/1, так как другой порт*

## Шаг 2. 

<img width="618" height="630" alt="image" src="https://github.com/user-attachments/assets/85ca2167-47d7-47c4-9bbe-83d3747563f9" />

*В каждом роутере создаём сообщение дня, роутеры R1,R2,R3 аналогично*

## Шаг 3.

<img width="1669" height="616" alt="image" src="https://github.com/user-attachments/assets/506a8556-9fe9-47d7-984c-5f72a0a33de7" />

*Переименовываем все устройства по шаблону нажав на утройство, далее вкладка Config→Global Settings, далее Display Name*

## Шаг 4.

<img width="1113" height="1125" alt="image" src="https://github.com/user-attachments/assets/7caef748-f814-4792-866c-d1d3f9c9b5d2" />

*Далее раздаем доменные имена всем устройствам в москве и в новосибирске аналогично*

## Шаг 5. 

<img width="987" height="1001" alt="image" src="https://github.com/user-attachments/assets/fa430cb5-f78b-4732-a08b-b13fa6e3a45b" />

*Создали vlan на коммутаторах*

## Шаг 6.

<img width="1070" height="1089" alt="image" src="https://github.com/user-attachments/assets/9f0f8023-2f8b-45df-9761-48bc7f685e6f" />

*Sw0*
<img width="1085" height="1025" alt="image" src="https://github.com/user-attachments/assets/d55eb775-805d-4e9e-a20f-650a7c20c6dd" />

*Sw1*

*Назначиваем порты в созданных Vlan-ах*

## Шаг 7.

<img width="1034" height="1029" alt="image" src="https://github.com/user-attachments/assets/fe4f8497-3592-464c-b71c-e2e3bab5a2e0" />

*Создаем канал EtherChannel 2-го уровня*

## Шаг 8.

<img width="702" height="713" alt="image" src="https://github.com/user-attachments/assets/e1ca7b00-4615-4829-ace4-5cdf69e306a8" />

*Создали Management interface на SW0 (rus-nsk-sw0)*

## Шаг 9.

<img width="701" height="711" alt="image" src="https://github.com/user-attachments/assets/3e586ff2-bc64-464e-b906-a2dab808c4f3" />

*Создали Management interface на SW1 (rus-nsk-sw1)*

## Шаг 10.

<img width="700" height="840" alt="изображение" src="https://github.com/user-attachments/assets/a6b5b1fa-f4ec-42d6-a90f-111dc714eb24" />

*Настройка SSHv2 на коммутаторах Новосибирска на rus-nsk-sw0*

<img width="702" height="747" alt="изображение" src="https://github.com/user-attachments/assets/959cfcc1-7b7e-484e-b8a0-f3b05fb254e1" />

*На rus-nsk-sw1*

## Шаг 11.

<img width="702" height="707" alt="изображение" src="https://github.com/user-attachments/assets/4f5b4fcb-7e15-4a02-8771-ff22c21433bb" />

*Настройка транка на f0/24 (rus-nsk-sw0)*

## Шаг 12.

<img width="697" height="351" alt="изображение" src="https://github.com/user-attachments/assets/03338853-ed90-4e58-b1cf-88015fbcbeff" />

*На rus-nsk-sw0*

<img width="699" height="273" alt="изображение" src="https://github.com/user-attachments/assets/feec2da2-1b64-4f63-9cf5-bd1cafcf7d92" />

*На rus-nsk-sw1*

## Шаг 13.

<img width="701" height="1003" alt="изображение" src="https://github.com/user-attachments/assets/0e630c76-bb19-4b5a-be91-42c0c688aa84" />

*Настройка портов f0/2, f0/3, f0/4 на rus-nsk-sw0*

<img width="688" height="760" alt="изображение" src="https://github.com/user-attachments/assets/0ab6b191-962c-47ac-925b-3709b865e040" />

*Настройка портов f0/2, f0/3, f0/4 на rus-nsk-sw1*

## Шаг 14. 

<img width="703" height="291" alt="изображение" src="https://github.com/user-attachments/assets/9becb5e2-bcbc-4ffa-8ecc-d06bec739c92" />

*Защита консольного подключения. На ОБОИХ коммутаторах, на SW1 точно также*

## Шаг 15. 

<img width="702" height="354" alt="изображение" src="https://github.com/user-attachments/assets/7166aa00-5108-414a-b13e-3e70662410c6" />

*Отключение exec timeout. На ОБОИХ коммутаторах, на SW1 точно также*

## Шаг 16. 

<img width="691" height="248" alt="изображение" src="https://github.com/user-attachments/assets/9618d220-278f-45d6-a658-0919da0faa9a" />

*Отключение логирования на консоль. На ОБОИХ коммутаторах, на SW1 точно также*

## Шаг 17. 

<img width="696" height="301" alt="изображение" src="https://github.com/user-attachments/assets/0fdd0065-bf01-4d7f-be7c-de13a3c6e15a" />

*Изменение размера буфера истории. На ОБОИХ коммутаторах, на SW1 точно также*

# Часть 2.

## Шаг 1.

<img width="689" height="216" alt="изображение" src="https://github.com/user-attachments/assets/5de2fe2c-11a7-4a56-93a6-07fb9de435f8" />

*Настраиваем IP-адрес на f0/1 на маршрутизаторе R1*

## Шаг 2. 

<img width="699" height="1037" alt="изображение" src="https://github.com/user-attachments/assets/7fea2338-73ee-4336-aee9-348fc20331e9" />

*Межсетевая маршрутизация (Router-on-a-Stick). Мы создаем виртуальные интерфейсы (субинтерфейсы) для каждого VLAN на порту, который смотрит в сторону SW0 (допустим, это FastEthernet0/0).*

## Шаг 3.

<img width="689" height="509" alt="изображение" src="https://github.com/user-attachments/assets/ace18372-d87e-4c14-afb9-42bc9a05cd24" />

*Настройка R1. Настройка DHCP-сервера. Создаем пулы адресов для каждого VLAN*

## Шаг 4. 

<img width="683" height="416" alt="изображение" src="https://github.com/user-attachments/assets/7a2c35ad-e31f-4207-ad0c-2625af15f551" />

*Пингуем с PC0*

# Часть 3.

## Шаг 1.

<img width="705" height="251" alt="изображение" src="https://github.com/user-attachments/assets/0865b3f1-d570-408b-bb99-886a65f49cfb" />

*Настроили имя многоуровневого коммутатора*

## Шаг 2.

<img width="700" height="215" alt="изображение" src="https://github.com/user-attachments/assets/d287bd96-5797-4980-a6d8-46fe04c09d3c" />

*Включили машрутизацию*

## Шаг 3.

<img width="698" height="283" alt="изображение" src="https://github.com/user-attachments/assets/124f86d8-2f47-46b0-8114-72a651761b18" />

*Создаем VLAN 100 и 200 с именами.*

## Шаг 4.

<img width="703" height="624" alt="изображение" src="https://github.com/user-attachments/assets/b22ebfa0-2825-4c3a-8ff4-9db2977c5b90" />

*Назначение интерфейсов*

## Шаг 5.

<img width="690" height="524" alt="изображение" src="https://github.com/user-attachments/assets/040c524e-112d-47ce-8132-0ba15682017e" />

*Настройка SVI на MLS*

## Шаг 6. 

<img width="679" height="545" alt="изображение" src="https://github.com/user-attachments/assets/5cab866d-c337-436e-9110-aba6f50daf6a" />

*Настройка интерфейсов 3-го уровня*

## Шаг 7. 

<img width="707" height="715" alt="изображение" src="https://github.com/user-attachments/assets/7daf56ee-b40e-4f52-a38e-24b60b803448" />

*Пингуем с PC6*

# Часть 4.

## Шаг 1.

<img width="703" height="361" alt="изображение" src="https://github.com/user-attachments/assets/2fdd0910-beec-4a03-aa28-629bd4317efc" />

*Настройка машрутизатора R2.*

## Шаг 2. 

<img width="701" height="377" alt="изображение" src="https://github.com/user-attachments/assets/d1619aac-0fe7-4cb9-b97f-44701599aee0" />

*Настройка R3*

## Шаг 3.

<img width="666" height="411" alt="image" src="https://github.com/user-attachments/assets/90abf907-483d-4668-9125-b3d347d39747" />

*Протокол резервирования R2*

<img width="708" height="371" alt="image" src="https://github.com/user-attachments/assets/8f5d9bfc-bb88-4336-b59b-08fb90a9a937" />

*R3 как резервный*

# Часть 5. 

## Шаг 1. 

<img width="709" height="436" alt="image" src="https://github.com/user-attachments/assets/1ef2fb6c-1c9b-4ace-b479-a2e9c7eb3054" />

*Настройка EIGRP на R1 nsk*

<img width="700" height="708" alt="image" src="https://github.com/user-attachments/assets/2165f958-e788-43ca-999d-889bb7c60f44" />

*Настройка EIGRP на R2 msk*

<img width="706" height="707" alt="image" src="https://github.com/user-attachments/assets/9629f1c7-60a2-4e16-881f-afbf90e20f15" />

*Настройка EIGRP на R3 msk*

<img width="705" height="718" alt="image" src="https://github.com/user-attachments/assets/c62c825b-9288-4385-b892-2ed3970be233" />

*Настройка EIGRP на MLS msk*

## Шаг 2.

<img width="700" height="965" alt="image" src="https://github.com/user-attachments/assets/c590158b-590d-47e3-aae1-afdff60a4b5f" />

*Настройка SSH на SW2*

<img width="700" height="895" alt="image" src="https://github.com/user-attachments/assets/f862cb98-6fcb-46f4-add7-5009dbc271dc" />

*Настройка SSH на SW1*

## Шаг 3.

<img width="705" height="711" alt="image" src="https://github.com/user-attachments/assets/9a8ecc17-a0ec-4c64-84d7-03cda50d4f0d" />

*Пропинговка с сервера*

#Часть 6 

## Шаг 1.

<img width="701" height="700" alt="изображение" src="https://github.com/user-attachments/assets/7660bf53-9f63-48d9-a787-834611a35960" />

*Ограничиdftv SSH на SW2 только с 10.0.0.100 и 2.0.0.100*

## Шаг 2.

<img width="701" height="709" alt="изображение" src="https://github.com/user-attachments/assets/9f8a2058-655b-4c4c-86d6-219dde014f85" />

*Разрешаем доступ к веб-серверу только с PC 2.0.0.100, на rus-msk-mls1*

## Шаг 3.

<img width="703" height="709" alt="изображение" src="https://github.com/user-attachments/assets/1973ca41-91a2-4a4d-a6d7-177b9bcf7753" />

* R2 и R3 могут пинговать всех, но НЕ ОТВЕЧАЮТ на пинги, на R2*

<img width="703" height="709" alt="изображение" src="https://github.com/user-attachments/assets/ea27f2d6-af25-4aa1-8ae5-a3da8ef8473f" />

*На R3*

<img width="701" height="713" alt="изображение" src="https://github.com/user-attachments/assets/f44a80d5-cd71-40d5-b27a-03ed0f44dddd" />

*Не пингуется*

# Часть 7

## Шаг 1-2.

<img width="706" height="713" alt="изображение" src="https://github.com/user-attachments/assets/602518e5-087b-49b5-bd8a-0da126087034" />

*Создаем loopback интерфейсы, на R1 (rus-nsk-r1)*

<img width="698" height="712" alt="изображение" src="https://github.com/user-attachments/assets/f69757f7-bdfd-4eaa-84c7-5b64ef66cc2d" />

*На R3 (rus-msk-r3)*

## Шаг 3-4.

<img width="702" height="716" alt="изображение" src="https://github.com/user-attachments/assets/f892427a-99b5-46ad-b17e-c27a6967195c" />

*Настраиваем RIPv2 ТОЛЬКО на R1 и R3, на R1*

<img width="703" height="712" alt="изображение" src="https://github.com/user-attachments/assets/6a039234-fc3c-44c3-bccb-23b6aaf68cab" />

*На R3*

## Шаг 5.

<img width="700" height="711" alt="изображение" src="https://github.com/user-attachments/assets/9818ee1c-46d2-4448-86b9-3cfcd3f84daf" />

*Настраиваем GRE туннель, на R1*

<img width="700" height="712" alt="изображение" src="https://github.com/user-attachments/assets/4f66096e-a010-4017-8e33-116c44b1e4c4" />

*На R3*

## Шаг 6.

<img width="706" height="715" alt="изображение" src="https://github.com/user-attachments/assets/6aa24ca1-685d-4bb9-ab6d-5435df116c7a" />

*Используем расширенный пинг для проверки*

# Часть 8.

## Шаг 1. 

<img width="706" height="713" alt="изображение" src="https://github.com/user-attachments/assets/8e6cda72-66eb-4d60-b418-e4cda3e6a3fe" />

*Настройка сервисов NTP и Syslog на R1*

<img width="702" height="707" alt="изображение" src="https://github.com/user-attachments/assets/7b52ee35-8f40-403c-9c98-a3ca52793c1c" />

*Настройка сервисов NTP и Syslog на R2*

<img width="693" height="708" alt="изображение" src="https://github.com/user-attachments/assets/d1420c9d-7b96-4ef1-b3ec-6203869126b9" />

*Настройка сервисов NTP и Syslog на R3*

<img width="701" height="716" alt="изображение" src="https://github.com/user-attachments/assets/34c238c2-7fac-4398-b7cd-bc2da48fceea" />

*Настройка сервисов NTP и Syslog на MLS*

## Шаг 2.

<img width="705" height="712" alt="изображение" src="https://github.com/user-attachments/assets/ba760189-5d9c-4790-9889-adc3870c7684" />

*Настройка SNMP на R2*

<img width="701" height="704" alt="изображение" src="https://github.com/user-attachments/assets/a21f5546-1089-4ef5-ab7b-e33b350f4a2b" />

*Настройка SNMP на R3*

## Шаг 3.

<img width="707" height="720" alt="изображение" src="https://github.com/user-attachments/assets/4c9258aa-59c7-4056-afb4-d0a2296cda8b" />

*Telnet с AAA на R3*

## Шаг 4. 

<img width="704" height="718" alt="изображение" src="https://github.com/user-attachments/assets/e297fb5c-d5ed-45f6-b4ca-a338b62470bd" />

*Настройка FTP на R2*

## Шаг 5.

<img width="703" height="715" alt="изображение" src="https://github.com/user-attachments/assets/bac68ccb-ffa9-4f5e-a2dc-8ab14ce99606" />


*Копирование конфигурации R2 на FTP сервер*

## Шаг 6.

<img width="704" height="712" alt="изображение" src="https://github.com/user-attachments/assets/9429487f-f258-4b03-a561-938cf977694f" />

*Отправить копию конфигурации R3 на сервер, используя протокол TFTP*

## Шаг 7.

<img width="699" height="741" alt="изображение" src="https://github.com/user-attachments/assets/eb44ab29-2bee-4d22-9d7f-3d6da509bbdb" />

*Проверка команд boot system на R3*

## Шаг 8.

<img width="698" height="718" alt="изображение" src="https://github.com/user-attachments/assets/96e29ddf-eabd-49f8-933b-960c4a312ba9" />


*Проверка Telnet с R2 на R3*

## Шаг 9.

<img width="719" height="738" alt="изображение" src="https://github.com/user-attachments/assets/c196f1dd-4ff6-4787-a08e-a5ef7dad48e0" />

*Смена пароля*



























