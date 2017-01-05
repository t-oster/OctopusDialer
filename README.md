# OctopusDialer
Lässt Systemtelefone an einer Octopus F/HiPath 3000 Telefonanlage Nummern wählen

ACHTUNG: Dieses Programm kann möglicherweise Ihre Telefonanlage beschädigen oder die Garantie einschränken. Es wird KEINERLEI Haftung jeglicher Art übernommen.

Ich setze dieses Programm erfolgreich ein, um in einer Umgebung mit Octopus F Telefonanlage Anrufe zu starten.  
rufe das Programm wie folgt auf:

```
java -jar OctopusDialer.jar <ip> <port> <src> <dst>
```

Damit wird die Telefonanlage unter <ip> und <port> (meistens 7001) kontaktiert und das Telefon mit der internen Durchwahl <src> ruft die Nummer <dst> an. Getestet
mit Siemens Open Stage T 40.

Ich kann nicht sagen, ob es nur mit unserer Anlage funktioniert, oder was genau das Programm tut. Ich habe lediglich mit Wireshark
einen Aufruf des Windows Wählhilfeprogramms (bei installiertem TAPI Treiber) aufgezeichnet und diese Kommunikation
nachgestellt.

Dann habe ich herausgefunden an welchen Stellen die Zielrufnummer und deren Länge übermittelt wird und habe diese angepasst.
Ich kann nicht sagen, ob es für alle Nummern funktioniert und welche Seiteneffekte es hat, aber bei uns geht's.

Download: https://github.com/t-oster/OctopusDialer/raw/master/release/OctopusDialer.jar

Viel Spaß
