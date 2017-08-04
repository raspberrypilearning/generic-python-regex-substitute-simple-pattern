- You can find and replace simple sequences of characters using Python's `re` module.

- A simple pattern would be a single character or sequence of characters, such as `A` or `cat`.

- First, import the `re` module into your script:

```python
import re
```

- Then create a simple string that you want to experiment with.

```python
import re
title = 'Harry Potter'
```

- Using `re.sub` you can change any character you like. For instance, changing the `r` character's to `i`, would look like this:

```python
new_title = re.sub(r'r', 'i', title)
print(new_title)
```
- This would give us `'Haiiy Pottei'.

- Note that first `r` that is outside of the quotes. This tells python than any string inside the quotes is a **literal** string, and to ignore special characters. You can see the difference by trying to type the following in an interpreter:

	```python
	print(r'Hello/nHello')
	print('Hello/nHello')
	```

- You can also change sequences of characters.

```python
new_title = re.sub(r'rr', 'pp', title)
```

- Printing `new_title` would now give you `'Happy Potter'`.

- You can also stop the substitution after a set number of replacements. So to only replace the first match, you could do this:

```python
new_title = re.sub(r'r', 'i', title, 1)
```

- Which would make the `new_title` `'Hairy Potter'`.
