## Algoritma Menentukan bilangan ganjil dan genap

1. Mulai
2. Masukan Bilangan yang ingin di periksa
3. Periksa apakah bilangan % 2 == 0
4. Jika ya, maka tampilkan: "Bilangan Genap"
5. Jika tidak, maka tampilkan: "Bilangan Ganjil"
6. Selesai

## Flowchart

```mermaid
flowchart LR
A@{shape : circle , label: "start"}
B@{shape : lean-r  , label: "X"}



A((Start)) --> B[/X?/]-->

C{X % 2 == 0} --TRUE--> D[/Even/]

C --FALSE--> E[/Odd/]

D & E --> F@{shape: dbl-circ, label: "End"}

```
