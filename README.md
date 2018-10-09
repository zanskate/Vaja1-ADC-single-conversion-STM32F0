# Vaja1-ADC-single-conversion-STM32F0
S pomočjo CUBE MX in Hal knjižnjicami v μVision 5 sprogramiramo mikroprocesor tako, da bo izvedel posamične ADC pretvorbe z izbranim potenciometrom.

ODGOVORI:
b) Glede na vašo razvojno ploščico in razširitveno vezje z tipkami ter potenciometri, izberite ustrezni
analogni vhod. Kateri pin je to? PCO

c) V Pinout zavihku ugotovite, koliko ADC pretvornikov ima vaša razvojna ploščica? 1
d) Izbrani ADC pretvornik ima oznako s trikotnikom. Kaj to pomeni?
Da je določen pin zaseden.

Kaj morate storiti, da razrešite to omejitev? Opišite in jo odpravite.
Pod zavihkom ADC obkljukamo željeni pin (PC0=IN10).

e) Razširite razdelek ADC. Koliko je vseh vhodnih kanalov? 17

f) Glede na potenciometer na vaši ploščici izberite-obkljukajte ustrezni kanal/pin. Na zaslonu se vam mora usterzno pobarvati izbrani pin v zeleno barvo. Kaj se izpiše poleg pina? ADC_IN10

h) V Configuration kliknemo ADC gumb. V Parameter settings izberite ločljivost pretvorbe na 8-bitno, torej je območje vrednosti od 0 ÷ 255. Kakšne so še ostale možne ločljivosti pretvorbe in območja vrednosti?
a) 12 bitno, od 0 do 4095,
b) 10 bitno, od 0 do 1023,
c) 6 bitno, od 0 do 63.



KOMENTAR NA DELOVANJE:
S pomočjo potenciometra in ADC pretvornika smo naredili program, ki nam izpisuje vrednost na potenciometru. S pomočjo Debug mode v μVision5 smo lahko na računalniku opazovali to vrednost. Pretvorba je 8 bitna, kar nam omogoča, da izpisuje vrednosti od 0 do 254. Pri nas nam vrne najvišjo vrednost 252 (slabši stik na potenciometru).
