# Geometrie Computațională - Stupariu

## Cursuri

- poate cel mai bun [website](http://gta.math.unibuc.ro/stup/geom_comp.html) de curs din facultate

## Subiecte

- [model de examen](https://www.dropbox.com/s/6bhl9zj8r887l64/231-geom-comp-exam.txt?dl=0)
- [model de examen](https://www.dropbox.com/sh/2pr9ofq998vgyq0/AADaMvUwXA_VLOYZBVG8V-1Ua?dl=0) via Iulia Duta

## Detalii despre examen (via Omulet Enervant)

Detalii despre examenul la Geometrie Computationala, seria 24:
Again, nu garantez ca sunt corecte sau ca proful nu se razgandeste.

Evaluare:
examenul valoreaza 60p
49 puncte finale(oficiu + lab + proiect lab + examen) = 4

cu cartile pe masa
orice notite, carte, suport de curs
e voie cu leptop, dar nu net, etc etc
NU LUCRAREA COLEGULUI SAU CIORNA COLEGULUI PE MASA
LUCRARE ORIGINALA, insista pe asta profu'
Daca descopera copiat, se enerveaza, studiaza, etc
O sa aiba harta salii, chiar sa nu copieze

timp de lucru: 1h 30

Subiecte:

1(5p). Aplicatie elementara din capitolul 1( raport, produs vectorial, test de orientare)
Ceva in genul exercitiilor din suportul de curs

2(10p) si 3(10p). Subiecte elementare legate de algoritmii prezentati( formulari directe sau "dati exemple")
Sectiunile de exercitii din suportul de curs

Gata cu chestii elementare.

4(10p). Complexitatea algebrica. Cat de complexe sunt calculele daca vreau sa rezolv nu stiu ce problema?

In R^2 sunt date 3 drepte prin ecuatiile lor generale. Care este complexitatea algebrica a calculelor daca dorim:
a. sa stabilim daca cele 3 drepte au exact 1 punct comun
b. presupunand ca a. e verificata, sa gasim coordonatele punctului de intersectie

Rezolvare:
a. ecuatie generala:
d: ax + by + c = 0
d': a'x + b'y + c' = 0
d'': a''x + b''y + c'' = 0

conditia de concurenta: sistemul de ecuatii (d, d', d'') e compatibil( AKA determinant {{a,b,c},{a',b',c'},{a'',b'',c''}}= 0) si admite exact 1 solutie
=> polinoame <= grad 3

b. punctul de intersectie este solutie a sistemului d, d' care e pol 2/ pol 2

5(10p). Complexitate timp/spatiu

De justificat(scurt, concis, la obiect, clar, etc) complexitatea timp/spatiu pentru:

a. un algoritm discutat la curs
b. un anume pas/pasi ai unui algoritm din suportul de curs
c. o metoda indicata explicit in subiect

Exemple:
a. Explicati de ce Graham's Scan are complexitatea O(n*log(n))
- e nevoie de preprocesare( ordonare) care consuma O(n*log(n))
- inserare 1 singura data in bucla principala
- stergere cel mult 1 data
=> complexitate O(n*log(n))

b. Care este complexitatea pasului 2 din algoritmul DeterminaDrum?
- O log(n) pentru ca se foloseste algoritmul de localizare pentru harti trapezoidale( complexitate timp mediu)

c. Fie P un poligon cu n varfuri. Explicati cum poate fi gasita acoperirea convexa in timp liniar adaptand Graham's Scan.
- argumente similare cu cele de la Graham's Scan

6(15p). "Algoritm"/"Problema cu parametri"

Transferul unei probleme geometrice intr-un algoritm

Exemplu:
Fie A(0,0), B(2,0), C(0,2) si D(alfa, alfa) cu alfa real.
Scrieti un algoritm care sa indice varfurile acoperirii convexe si ca calculeze coordonatele centrului de greutate al poligonului asociat.

Se puncteaza:
- realizarea figurii si sa realizam ca D e pe prima bisectoare(din cauza ca e alfa, alfa)
- intelegerea contextului geometric
- calcule geometrice( calcule complicate = subiect gresit sau am gresit noi)

alfa < 0: acoperirea convexa (B, C, D) cu gentrul de greutate( (alfa + 2) / 3, (alfa + 2) / 3)
alfa = 0: caz degenerat ( D = A) cu acoperirea convexa (B, C, D = A) cu centrul de greutate( 2/3, 2/3)
alfa in (0,1): acoperirea convexa (A, B, C) cu centrul de greutate( 2/3, 2/3)
alfa = 1: caz degenerat( D apartine [BC]) cu acoperirea convexa (A, B, C) cu centrul de greutate( 2/3, 2/3)
alfa > 1: acoperirea convexa A, B, C, D cu centrul de greutate( (afla + 2) / 4, (afla + 2) / 4)

Pentru cazurile degenerate daca D = A => 2 puncte coinccid
daca D e pe [BC], D se afla pe frontiera acoperirii convexe, dar nu e varf al sau

Se puncteaza analiza cazurilor degenerate + interpretarea geometrica

Algoritmul:
INPUT: alfa
CALCULE/ OUTPUT: cod/ pseudocod/ poveste

Se puncteaza selectarea corecta a inputului.

In principiu rezultatele se dau in aceisai zi. Eventual sa se si discute. O sa se anunte la fiecare grupa( rezultate azi la X, pe net, etx)