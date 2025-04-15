# Algoritma Menentukan suhu Celsius (C), Farenheit (F), Reamur (R), dan Kelvin(K)

1. Mulai

2. Masukkan suhu dalam satuan Celsius (C)
3. Pilih Type :
4. Jika Type "F" Hitung Fahrenheit (F) dengan rumus:
   → F = (C × 9/5) + 32

5. Jika Type "R" Hitung Reamur (R) dengan rumus:
   → R = C × 4/5

6. Jika Type "K" Hitung Kelvin (K) dengan rumus:
   → K = C + 273.15

7. Tampilkan hasil suhu dalam satuan Fahrenheit, Reamur, dan Kelvin

8. Selesai

# PSEUCODE

```
DECLARE Calcius :REAL
DECLARE Kelvin REAL
DECLARE Farenheit : REAL
DECLARE Reamur : REAL
DECLARE Type : CHAR
DECLARE Result : REAL
INPUT Calcius
INPUT Type
IF Type == "K"
   Result <- Calcius + 23
ENDIF
IF Type == "F"
   Result <- (9/5 x Calcius) + 32
ENDIF
IF Type == "R"
   Result <- 4/5 x Calcius
ENDIF

OUTPUT RESULT
```

# FLOWCHART

```mermaid
flowchart TD
  A@{ shape: circle, label: "Start" }
  Isnumber@{ shape: diamond , label: "C !== NUMBER" }
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
Isnumber --False--> B
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
