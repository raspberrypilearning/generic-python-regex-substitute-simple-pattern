- You can find and replace simple patterns of characters using Python's `re` module.

- A simple pattern would be a single character or a sequence of characters, such as 'A' or 'cat'.

- First, import the `re` module in your script:

```python
import re
```

- Then create a simple string with which to experiment.

```python
import re
title = 'Harry Potter'
```

- Using `re.sub` you can change any character in the string. For instance, changing the `r` characters to `i` looks like this:

```python
new_title = re.sub('r', 'i', title)
print(new_title)
```
- This will give us `'Haiiy Pottei'`.

- You can also change sequences of characters:

```python
new_title = re.sub('rr', 'pp', title)
```

- Printing `new_title` will now give you `'Happy Potter'`.

- Of course, you can also substitute whole words.

```python
new_title = re.sub('Potter', 'Styles', title)
```

- You can also stop the substitution after a set number of replacements. So to only replace the first match, you can do this:

```python
new_title = re.sub('r', 'i', title, 1)
```

- This will make the `new_title` variable contain `'Hairy Potter'`.
