- Je kunt eenvoudige patronen van tekst vinden en vervangen met behulp van de `re` module van Python.

- Een eenvoudig patroon zou een enkel karakter of een reeks karakters zijn, zoals 'A' of 'kat'.

- Importeer eerst de `re` module in je script:

```python
import re
```

- Maak vervolgens een eenvoudige string waarmee je kunt experimenteren.

```python
import re
titel = 'Harry Potter'
```

- Met behulp van `re.sub` kun je elk teken in de tekenreeks wijzigen. Als je bijvoorbeeld de `r` letters wijzigt in `i` dan ziet dit er als volgt uit:

```python
nieuwe_titel = re.sub('r', 'i', titel)
print(nieuwe_titel)
```
- Dit geeft ons `'Haiiy Pottei'`.

- Je kunt ook reeksen tekens wijzigen:

```python
nieuwe_titel = re.sub('rr', 'pp', titel)
```

- Als je `nieuwe_titel` afdrukt, krijg je nu `'Happy Potter'`.

- Je kunt natuurlijk ook hele woorden vervangen.

```python
nieuwe_titel = re.sub('Potter', 'Styles', titel)
```

- Je kunt de vervanging ook stoppen na een bepaald aantal vervangingen. Dus om alleen de eerste overeenkomst te vervangen, kun je dit doen:

```python
nieuwe_titel = re.sub('r', 'i', titel, 1)
```

- Hierdoor bevat de variabele `nieuwe_titel ` `'Hairy Potter'`.
