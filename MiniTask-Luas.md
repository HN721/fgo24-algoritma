# Algoritma Menentukan suhu Celsius (C), Farenheit (F), Reamur (R), dan Kelvin(K)

1. Mulai

2. Masukkan suhu dalam satuan Celsius (C)

3. Hitung Fahrenheit (F) dengan rumus:
   → F = (C × 9/5) + 32

4. Hitung Reamur (R) dengan rumus:
   → R = C × 4/5

5. Hitung Kelvin (K) dengan rumus:
   → K = C + 273.15

6. Tampilkan hasil suhu dalam satuan Fahrenheit, Reamur, dan Kelvin

7. Selesai

# PSEUCODE

```
DECLARE CALCIUS :REAL
DECLARE KELVIN REAL
DECLARE FARENHEIT : REAL
DECLARE REAMUR : REAL

INPUT
KELVIN <- CALCIUS + 273
FARENHEIT <- (9/5 X CALCIUS) + 32
REAUMUR  <-  4/5 X CALCIUS
OUTPUT " HASIL KONVERSI SUHU C KE K ADALAH ",KELVIN
OUTPUT " HASIL KONVERSI SUHU C KE F ADALAH " , FARENHEIT
OUTPUT "HASIL KONVERSI SUHU C KE R ADALAH " ,REAMUR

```

# FLOWCHART

```mermaid
flowchart TD
  A@{ shape: circle, label: "Start" }
  Isnumber@{ shape: lean-r , label: "C !== NUMBER" }
  type@{ shape: lean-r , label: "input:type" }

  type1@{ shape: diamond , label: "Type: F" }
  type2@{ shape: diamond , label: "Type: k" }
  type3@{ shape: diamond , label: "Type: R" }
  output@{shape: lean-r, label: "Output : Result"}
  B@{shape: lean-r, label: "C?"}
  C@{shape , label: "Result = (C × 9/5) + 32"}
  D@{shape , label: "Result = C × 4/5"}
  E@{shape , label: "Result = C + 273.15"}
  H@{shape: dbl-circ, label: "End"}
A --> B
B --> Isnumber
Isnumber --> type
type --> type1
type1 --TRUE--> C
type1 --False--> type2
type2 --True--> D
type2 --False--> type3
type3 --True--> E
type3 --False--> H
C --> output
D --> output
E --> output

output --> H





```
