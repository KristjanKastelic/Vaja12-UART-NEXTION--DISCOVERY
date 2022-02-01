# Vaja12-UART-NEXTION--DISCOVERY

Dodajte grafični kazalec (gauge) iz okna Toolbox na vaš Display. Ustrezno ga povečajte in
pozicionirajte/centrirajte ter nastavite barvo in debelino kazalca (wid, pco). Po želji mu lahko nastavite
prosojnost (sta → solid color/crop). Kako je Nextion poimenoval ta objekt (objname)? z0.

V oknu Events za gumb _b1_ (objname), v zavihku Touch Press Event prepišemo spodnjo kodo

V zavihku Pinout izbrišite (reset state) trenutne privzete postavite pinov - razen za LED diodi, ki imata
vrednost _PA5_ (zelena LED)

Aktivirana pina _PA1_ (Rx) in _PA0_ (Tx) pravilno povežite z Nextionom! Kako? Utemeljite: _TX vežemo na RX in RX na TX._

Kateri kanal morate izbrati? _PC0_.

V zgornjih vrsticah smo aktivirali ADC pretvorbo – katera vrsta pretvorba je to? (single, continous ali časovno
sprožena?) Odg. _SINGLE_.

ascii    bin       dec   hex 
o        00110000  48   30   
1        00110001  49   31  
2        00110010  50   32
3        00110011  51   33
4        00110100  52   34
5        00110101  53   35
6        00110110  54   36
7        00110111  55   37
8        00111000  56   38
9        00111001  57   39

Kaj pa
pomeni 3x zapis 0xff? _0xff je zaključek komande._.
Kakšen ASCII znak prejme Nextion? _NUL_ .

Komentar: največ težav sem imel z nextionom saj mi je javljal napake, ki sem jih razrešil. V nalogi mi deluje vse razen ne prižge se LED.
