## Algoritma Menentukan bilangan ganjil dan genap

1. Mulai
2. Masukan Bilangan yang ingin di periksa
3. Periksa apakah bilangan % 2 == 0
4. Jika ya, maka tampilkan: "Bilangan Genap"
5. Jika tidak, maka tampilkan: "Bilangan Ganjil"
6. Selesai

## Pseudocode

```
DECLARE Bilangan : REAL
DECLARE Ganjil : REAL
DECLARE Genap : REAL
INPUT Bilangan
IF  Bilangan % 2 == 0 THEN
    Genap <- Bilangan
    OUTPUT "BILANGAN  GENAP :",Genap
ELSE
    Ganjil <- Bilangan
    OUTPUT "BILANGAN  GANJIL :",Ganjil
ENDIF
```

## Flowchart

```mermaid
flowchart LR
A@{shape : circle , label: "start"}
B@{shape : lean-r  , label: "X"}



A((Start)) --> B[/Bilangan/]-->

C{Bilangan % 2 == 0} --TRUE--> D[/'Bilangan Genap'/]

C --FALSE--> E[/'Bilangan Ganjil'/]

D & E --> F@{shape: dbl-circ, label: "End"}

```
