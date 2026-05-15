# Python Collections Guide 🚀

Python-এ data store করার জন্য সবচেয়ে common built-in containers হলো:

* **List**
* **Tuple**
* **Set**
* **Dictionary**

এগুলা অনেক time interview, problem solving, projects, database handling, API response processing—সব জায়গায় use হয়।

---

# 1. List `[]`

List হলো **ordered, mutable collection**

মানে:

* Order maintain করে
* Duplicate allow করে
* Value change করা যায়
* Different data types রাখতে পারে

```python
my_list = [1, 2, 3, "python", 5.5]

print(my_list)
```

### Features

✅ Ordered
✅ Mutable
✅ Duplicate allowed
✅ Indexing supported

---

### Common Methods

```python
append()
insert()
remove()
pop()
sort()
reverse()
clear()
copy()
extend()
```

---

### কখন List use হয়?

Use list when:

* Multiple values sequentially store করতে হবে
* Values frequently add/remove করতে হবে
* Indexing দরকার
* Ordered data দরকার

### Example:

* Student marks list
* Shopping cart items
* Todo list
* API response data

---

# 2. Tuple `()`

Tuple হলো **ordered, immutable collection**

মানে:

* Order maintain করে
* Duplicate allow করে
* Value change করা যায় না

```python
my_tuple = (1, 2, 3)

print(my_tuple)
```

---

### Features

✅ Ordered
❌ Mutable না
✅ Duplicate allowed
✅ Indexing supported

---

### Common Methods

```python
count()
index()
```

---

### কখন Tuple use হয়?

Use tuple when:

* Fixed data store করতে হবে
* Data accidental change prevent করতে হবে
* Faster performance দরকার

### Example:

* Coordinates `(x,y)`
* Database records
* RGB color values

```python
location = (23.7, 90.4)
```

---

# 3. Set `{}`

Set হলো **unordered, mutable collection of unique values**

মানে:

* Order guarantee নেই
* Duplicate allow করে না
* Unique values store করে

```python
my_set = {1, 2, 3, 4}

print(my_set)
```

---

### Features

❌ Ordered না
✅ Mutable
❌ Duplicate allowed না
❌ Indexing support নেই

---

### Common Methods

```python
add()
remove()
discard()
union()
intersection()
difference()
```

---

### কখন Set use হয়?

Use set when:

* Unique data দরকার
* Duplicate remove করতে হবে
* Fast membership checking দরকার

### Example:

* Unique usernames
* Unique tags
* Duplicate removal

```python
nums = [1,1,2,2,3]
print(set(nums))
```

---

# 4. Dictionary `{key:value}`

Dictionary হলো **key-value pair based collection**

```python
student = {
    "name": "Sakib",
    "age": 22
}
```

---

### Features

✅ Ordered (Python 3.7+)
✅ Mutable
❌ Duplicate keys allowed না
❌ Index based না

---

### Common Methods

```python
get()
keys()
values()
items()
update()
pop()
copy()
```

---

### কখন Dictionary use হয়?

Use dictionary when:

* Key দিয়ে data access করতে হবে
* Structured data store করতে হবে
* Real world object represent করতে হবে

### Example:

* User profile
* JSON data
* API response
* Database row

```python
user = {
    "name": "Rahim",
    "email": "rahim@gmail.com"
}
```

---

# List vs Tuple vs Set vs Dictionary

| Feature    | List | Tuple | Set  | Dictionary    |
| ---------- | ---- | ----- | ---- | ------------- |
| Syntax     | `[]` | `()`  | `{}` | `{key:value}` |
| Ordered    | ✅    | ✅     | ❌    | ✅             |
| Mutable    | ✅    | ❌     | ✅    | ✅             |
| Duplicates | ✅    | ✅     | ❌    | Keys ❌        |
| Indexing   | ✅    | ✅     | ❌    | ❌             |
| Key-Value  | ❌    | ❌     | ❌    | ✅             |

---

# কখন কোনটা use করবো?

### Use List → when order + modification needed

```python
cart = ["shirt", "shoe", "watch"]
```

---

### Use Tuple → when fixed data needed

```python
coordinate = (23.7, 90.4)
```

---

### Use Set → when unique values needed

```python
tags = {"python", "django", "flask"}
```

---

### Use Dictionary → when key-value mapping needed

```python
student = {
    "name": "Sakib",
    "id": 101
}
```

---

# Easy Memory Trick 😎

### List → Changeable box

### Tuple → Locked box

### Set → Unique box

### Dictionary → Labeled box

---

# Real Life Example

Imagine student data:

### List

সব subject marks

```python
[80, 90, 70]
```

---

### Tuple

Fixed birth date

```python
(12, "May", 2002)
```

---

### Set

Unique skills

```python
{"Python", "C++", "Java"}
```

---

### Dictionary

Full student profile

```python
{
    "name": "Sakib",
    "age": 22,
    "dept": "CSE"
}
```

---

# Final Rule 🔥

If confused:

* Need order? → List/Tuple
* Need modification? → List
* Need fixed data? → Tuple
* Need unique values? → Set
* Need key-value pair? → Dictionary

---


