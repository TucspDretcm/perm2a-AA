# Perm2a-Algebra Abstracta

**Integrantes:**

*   Gabriel Ivan Rodriguez Postigo
*   Jaime Mateo Gutiérrez Muñoz
*   Alexander Carpio Mamani

**Como correr el codigo:**
* Para poder ver y probar el trabajo selecione el archivo "perm2a.ipynb" y luego clickear en "Open in colab" para poder correr el programa.

**El mejor "s":**
* **El mejor "s" para correr el algoritmo es 3, fue encontrado haciendo 3 tipos de pruebas que se pueden encontran en el "perm2a.ipynb"**, pero en la prueba donde nos dimos cuenta que sufre más fue en:

```python
def GEN_PRIMO_SIGUIENTE(n, s):
  n = n + 1 - (n % 2)
  while MILLER_RABIN(n, s) == False:
    n = n + 2
  return n

numero_pruebas = 1000

for s in range(0, 20):   # probamos para "s" del 0 al 19.
  print("s: ", s, end="")

  parte = [GEN_PRIMO_SIGUIENTE(2, s)]
  for i in range(numero_pruebas - 1):
    parte.append(GEN_PRIMO_SIGUIENTE(parte[-1] + 1, s))

  primos = []
  for p in parte:
    if MILLER_RABIN(p, 100):    # evaluamos el número generado con un s=100 que es muy confiable
      primos.append(p)

  print("  generados:", len(primos))
```

**output:**
```
s:  0  generados: 302
s:  1  generados: 991
s:  2  generados: 998
s:  3  generados: 1000
s:  4  generados: 1000
s:  5  generados: 1000
s:  6  generados: 1000
s:  7  generados: 1000
s:  8  generados: 1000
s:  9  generados: 1000
s:  10  generados: 1000
s:  11  generados: 1000
s:  12  generados: 1000
s:  13  generados: 1000
s:  14  generados: 1000
s:  15  generados: 1000
s:  16  generados: 1000
s:  17  generados: 1000
s:  18  generados: 1000
s:  19  generados: 1000
```
