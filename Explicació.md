# PRÀCTICA 5: Sensor de temperatura i humitat
<div align="right">

**Clara Barba Armengol**
 </div>

<div align="justify">
Aquesta pràctica consisteix en un sensor de temperatura i humitat que mostra les dades per un display i a la vegada per una web asíncrona. 
</div>

## EXERCICI 1
El codi ens és proporcionat a la pràctica. El què fa és buscar tots els dispositiu I2C que hi ha conectats. Si no en troba cap mostra per pantalla *No I2C devices found*. Té un contador que calcula quants dispositius hi ha. El codi d'aquest exercici el podem trobar al repositori "Practica5_ex1".

## EXERCICI 2
Se'ns demana que realitzem un programa que utilitzi algun dispositiu I2C. En el meu cas he muntat un sensor de temperatura i humitat que mostra les seves dades per un display i també per una web asíncrona. El sensor de temperatura HTU21D està constantment llegint valors per tant la web ha de ser asíncrona per tal de que es vagi actualitzant en tot moment. 

## Material
- Sensor de temperatura i humitat HTU21D
- Display
- Cables 
- ESP32

## Muntatge 

<div align="justify">

 He muntat el dispositiu a una protoboard. He fet la següent assignació de pins:
 - SDA del display i DA del Sensor --> 21
 - CLK del SDA i del Sensor --> 22
 - VCC a 3.3V 

 No ha sigut necessari conectar cap resistència en sèrie. 
</div>

## Funcionament general

<div align="justify">

Quan es clica a *Upload and Monitor* i s'executa el programa ens apareix per pantalla la IP de la web. A continuació tant en la pantalla de l'ordinador com en el display podem anar veient com va variant la temperatura i la humitat en cada instant. Si escrivim la IP en el cercador podem accedir la web i veure també les dades que llegeix el sensor.
[Vídeo del funcionament](https://drive.google.com/file/d/13fZTZw2H7C8iWyex_wNAnhgZKgz-yB1D/view?usp=sharing).

La web que he creat té el següent aspecte: 
!(WEB)["/web.png"]
Aquests nombres apareixen com a dades quan el sensor no està conectat (com ara).
</div>
<div align="justify">
 
</div>
No he pogut realitzar els exercicis per pujar nota perquè no tinc el sensor d'oxigen en sang i freqüència cardíaca. 