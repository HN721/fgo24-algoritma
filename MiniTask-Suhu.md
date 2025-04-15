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
DECLARE CALCIUS :REAL
DECLARE KELVIN REAL
DECLARE FARENHEIT : REAL
DECLARE REAMUR : REAL
DECLARE TYPE : CHAR
DECLARE RESULT : REAL
INPUT CALCIUS

IF TYPE == "K"
   RESULT <- CALCIUS + 23
ENDIF
IF TYPE == "F"
   RESULT <- (9/5 x CALCIUS) + 32
ENDIF
IF TYPE == "R"
   RESULT <- 4/5 x CALCIUS
ENDIF

OUTPUT "HASIL KONVERSI ADALAH",RESULT
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
