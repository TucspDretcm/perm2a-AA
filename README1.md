Perm1c-AlgebraAbstracta

Para el ejercicio número 1:


Descripción del Algoritmo:
1) Generar todos los primos de 3, 4 y 5 cifras.
Comenzará desde la minima cifra que le demos, ejemplo, si queremos cifra de 3 lo que hará es 10**(3-1) lo cual es 100 siendo el minimo numero de 3 cifras.
Luego entra un bucle while que mientras que el número primo generado gracias a la funcion GEN_PRIMO, que genera el siguiente o el mismo primo a el número enviado o sea al anterior primo más 1, convertido en string y viendo la longitud de la cadena si es menor a 5 seguira generando numeros, donde cada número generado lo guardamos en una lista para luego imprimirla.


Hicimos dos pruebas con el "s";:

-La primera genera números primos no repetidos con el RANDOMGEN_PRIMOS con un "s" del 0 hasta el 100 y luego los evalua con la función MILLER_RABIN con un "s" de 100.
-La segunda prueba evalua cierto numeros de primos generados con un s de 100 y numeros no primos    random, los evalua con un MILLER_RABIN con "s" de 0 a 100