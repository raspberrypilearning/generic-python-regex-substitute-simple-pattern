- Puedes encontrar y reemplazar patrones simples de caracteres usando el módulo `re` de Python.

- Un patrón simple sería un único carácter o una secuencia de caracteres, tales como 'A' o 'gato'.

- Primero, importa el módulo `re` en tu script:

```python
import re
```

- Luego crea una cadena simple con la cual experimentar.

```python
import re
titulo = 'Harry Potter'
```

- Usando `re.sub` puedes cambiar cualquier carácter de la cadena. Por ejemplo, cambiar los caracteres `r` a `i` se ve así:

```python
nuevo_titulo = re.sub('r', 'i', titulo)
print(nuevo_titulo)
```
- Esto nos dará `'Haiiy Pottei'`.

- También puedes cambiar secuencias de caracteres:

```python
nuevo_titulo = re.sub('rr', 'i', titulo)
```

- Imprimir `nuevo_titulo` ahora te dará `'Happy Potter'`.

- Por supuesto, también puede sustituir palabras enteras.

```python
nuevo_titulo = re.sub('Potter', 'Estilos', titulo)
```

- También puedes detener la sustitución después de un número determinado de reemplazos. Así que para reemplazar solo la primera coincidencia, puedes hacer esto:

```python
nuevo_titulo = re.sub('r', 'i', titulo, 1)
```

- Esto hará que la variable `nuevo_titulo` contenga `'Hairy Potter'`.
