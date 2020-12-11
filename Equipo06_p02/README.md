# Parte 1.
### Pregunta 1-
**Tabla.**

# Parte 2.
### Pregunta 1-
**Usando awk o python, conviertan este archivo de fastq a fasta.**

Comando en la terminal:
~~~
sed -n '1~4s/^@/>/p;2~4p' ERR486827_2.fastq > ERR486827_2.fasta
~~~
### Pregunta 3-
**Obtengan el promedio de la longitud de las secuencias para cada archivo creando una función de python que haga la tarea.**
~~~
D = []
with open(A) as file_object:
      for l in file_object:
          if l[0] != '>':
             D.append(len(l))
E = sum(D)
F = 398824
Promedio = E / F
print(Promedio)
151.0
~~~
