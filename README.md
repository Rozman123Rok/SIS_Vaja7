# Kratko časovna Furierova transformacija in analiza signala DTMF

Demonstrirajte znanja Kratko časovne Fourierove transformacije z analizo vsebine podanega signala DTMF.

Pripravite Python skripto ki ima definirane (vsebuje) naslednje funkcije:

## def analiziraj_dtmf(signal, vzorcevalna_frekvenca, min_cas_ton, min_cas_pavza):

- funkcija prejme 4 parametre
  - funkcija prejme vektor (x, 1), v katerem se nahaja signal za dekodiranje
   - pravilno generirni DTMF ton ne bodo krajši kot 65ms
  - vzorčevalno frekvenco signala v hercih, ki pove koliko vzorcev na sekundo je v signalu
  - minimalni čas trajanja tona v milisekundah, ki pove minimalni čas, kateri mora biti DTMF ton prisoten da ga upoštevamo kot pravilnega
  - minimalni čas trajanja premora za tonom v milisekundah, ki pove minimalni čas "tišine", kateri mora biti prisotna da upoštevamo zaznan DTFM ton kot pravilen
- funkcija naj vrne vektor oblike (n, 1) za n prepoznanih vrednosti
  - prepoznane vrednosti vključujejo znake: *, #, 0, 1, 2, 3, 4, 5, 6, 7, 8 in 9
- (55 točk) - rezultat funkcije se točkuje glede na naslednje kriterije
  - 18 točk za pravilno dekodiranje v čistem in pravilno generiranem signalu
  - 9 točk za uspešno ignoriranje nepravilno generiranih tonov
  - 27 točk za odpornost na šum
   - 0-27 točk se razporedi glede na jakost šuma
     - 10 db nivo signala: + 2 točke
     - 5 db nivo signala: + 2 točke
     - 0 db nivo signala: + 2 točke
     - -2 db nivo signala: + 3 točke
     - -4 db nivo signala: + 3 točke
     - -6 db nivo signala: + 4 točke
     - -8 db nivo signala: + 5 točke
     - -10 db nivo signala: + 6 točke
Pripravite še odsek kode katero lahko lahko samostojno zaženete kot demo:

## if __name__ == '__main__':

- pripravite demo katerega lahko poženete
  - print("Modul za DTMF analozo!")
 

Zahtevano implementacijo oddajte v datoteki dtmfanaliza.py.