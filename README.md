# flink
#Teste ut Confluent Platform inkl. Confluent Flink på PC med QSL og Docker

#Starte WSL (Windows Subsystem for Linux):
#På ditt Windows 11-skrivebord, skriv PowerShell i søkefeltet, velg "Run as Administrator"
PS C:\Windows\system32> wsl

#Starte Flink:
cd /home/dahlto/cp-all-in-one/cp-all-in-one
sudo docker compose up -d

#FlinkSQL:
dahlto@v8-dell-p3520:~/cp-all-in-one/cp-all-in-one$ sudo docker exec -it flink-sql-client /bin/bash
#FlinkSQL CLI:
/opt/flink/bin/sql-client.sh

#Avslutte FlinkSQL CLI:
quit;

#Avslutte FlinkSQL:
exit

#Avslutte Flink:
sudo docker compose down

#Avslutte wsl:
exit

#Avslutte Powershell:
exit
