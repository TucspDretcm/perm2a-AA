Perm1c-AlgebraAbstracta

Para el ejercicio número 2:


Descripción del Algoritmo:
2) Implementar un programa que genere de manera aleatoria al menos 10 primos distintos de 16, 32 y 64 bits.
Para este programa usamos la funcion RANDOMGEN_PRIMOS la cual genera un número primo de acuerdo a la cantidad de bits enviada; en el algoritmo lo que hace es generar 10 número para 16, 32 y 64 bits, pero como es random algunos quizas se repetiran por eso usamos un if para ver que si el número generado con x bits no esta en la lista se agregue caso contrario vuelve a generar otro y asi se repite en el bucle hasta que la longitud de la lista sea mayor o igual a 10.


Hicimos dos pruebas con el "s";:

-La primera genera números primos no repetidos con el RANDOMGEN_PRIMOS con un "s" del 0 hasta el 100 y luego los evalua con la función MILLER_RABIN con un "s" de 100.
-La segunda prueba evalua cierto numeros de primos generados con un s de 100 y numeros no primos    random, los evalua con un MILLER_RABIN con "s" de 0 a 100