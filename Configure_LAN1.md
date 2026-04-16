#Часть 1
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




