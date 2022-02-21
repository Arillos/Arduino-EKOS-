## Informacje wstępne:

Przed przystąpieniem do zajęć warto zapoznać się z informacjami zawartymi w kursie Forbot odnośnie [instalacji Arduino IDE](https://forbot.pl/blog/kurs-arduino-srodowisko-jak-zaczac-programowac-id936).

## Cel zajęć:
1. Instalacja i konfiguracja środowiska Arduino IDE.
2. Omówienie platformy Arduino.
3. Instalacja wszystkich niezbędnych bibliotek potrzebnych do realizacji zajęć.
4. Implementacja pierwszego programu o nazwie Blink.

## Zadanie:
1. Zainstaluj środowisko Arduino IDE zgodnie wg [poradnika](https://forbot.pl/blog/kurs-arduino-srodowisko-jak-zaczac-programowac-id936) kursu Forbot.
2. Umieść w folderze libraries (ścieżkę dostępu poda nauczyciel) wszystkie biblioteki z folderu [!Biblioteki Arduino](https://github.com/Arillos/Arduino/tree/main/!Biblioteki%20Arduino).
3. Podłącz Arduino do komputera za pośednictwem przewodu USB A-B.
4. Podłącz czerwoną diodę LED do PINU 2.
5. Zweryfikuj i wgraj pierwszy program [Blink]().
6. Zmodyfikuj program z punktu 5. aby zasygnalizować diodą LED sygnał S.O.S.

## Schemat połączenia:


## Kod programu:
'''

// W funkcji SETUP umieszczamy wszystkie informacje początkowe
// niezbędne do uruchomienia programu np. czy dany PIN w Arduino
// (np. PIN 2) ma być traktowany jako WEJŚCIE (INPUT), czy WYJŚCIE
// (OUTPUT).

void setup()
{
  // Informujemy Arduino, że PIN 2 będzie wysyłać sygnał
  pinMode(2, OUTPUT);
}

// W funkcji LOOP znajduje się cały algorytm. Każda instrukcja
// wykonywana jest krok po kroku (linijka po linijce).

void loop()
{
  // Wysyłamy na PIN 2 stan WYSOKI (logiczne 1 - HIGH)	
  digitalWrite(2, LOW);
  //Odczekujemy 1 sekundę (1000 milisekund)
  delay(1000);
  // Wysyłamy na PIN 2 stan NISKI (logiczne 0 - LOW)
  digitalWrite(2, HIGH);
  //Odczekujemy 1 sekundę (1000 milisekund)
  delay(1000);  
}
'''


##. Rezultat:
Zrealizowany  skrypt prześlij na: ariel_antonowicz@ekos.edu.pl