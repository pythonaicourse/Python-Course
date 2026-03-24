📘 Python 30-Day Syllabus

# 📘 Day05 Notes

## 🔹 Type Casting

We can convert one type value to another type. This conversion is called **Typecasting** or **Type coercion**.

The following are various inbuilt functions for type casting:

1. `int()`
2. `float()`
3. `complex()`
4. `bool()`
5. `str()`

---

## 🔹 1. int()

We can use this function to convert values from other types to int.

```
>>> int(123.987)
123

>>> int(10+5j)
TypeError: can't convert complex to int

>>> int(True)
1

>>> int(False)
0

>>> int("10")
10

>>> int("10.5")
ValueError: invalid literal for int() with base 10: '10.5'

>>> int("ten")
ValueError: invalid literal for int() with base 10: 'ten'

>>> int("0B1111")
ValueError: invalid literal for int() with base 10: '0B1111'
```

### ✅ Note:

* We can convert from any type to int **except complex type**.
* To convert `str` → `int`, the string must contain **only integral values in base-10**.

---

## 🔹 2. float()

We can use `float()` function to convert other type values to float.

```
>>> float(10)
10.0

>>> float(10+5j)
TypeError: can't convert complex to float

>>> float(True)
1.0

>>> float(False)
0.0

>>> float("10")
10.0

>>> float("10.5")
10.5

>>> float("ten")
ValueError: could not convert string to float: 'ten'

>>> float("0B1111")
ValueError: could not convert string to float: '0B1111'
```

### ✅ Note:

* We can convert any type to float **except complex type**.
* String must be **integer or floating-point literal in base-10**.

---

## 🔹 3. complex()

We can use `complex()` function to convert other types to complex type.

### ▶ Form-1: `complex(x)`

Converts `x` into a complex number with imaginary part `0`.

```
complex(10) ==> 10+0j
complex(10.5) ==> 10.5+0j
complex(True) ==> 1+0j
complex(False) ==> 0j
complex("10") ==> 10+0j
complex("10.5") ==> 10.5+0j

complex("ten")
ValueError: complex() arg is a malformed string
```

### ▶ Form-2: `complex(x, y)`

`x` → real part, `y` → imaginary part

```
complex(10,-2) ==> 10-2j
complex(True,False) ==> 1+0j
```

---

## 🔹 4. bool()

We can use this function to convert other type values to boolean.

```
bool(0) ==> False
bool(1) ==> True
bool(10) ==> True
bool(10.5) ==> True
bool(0.178) ==> True
bool(0.0) ==> False
bool(10-2j) ==> True
bool(0+1.5j) ==> True
bool(0+0j) ==> False
bool("True") ==> True
bool("False") ==> True
bool("") ==> False
```

---

## 🔹 5. str()

We can use this method to convert other type values to string.

```
>>> str(10)
'10'

>>> str(10.5)
'10.5'

>>> str(10+5j)
'(10+5j)'

>>> str(True)
'True'
```

---

## 🔹 Fundamental Data Types vs Immutability

All fundamental data types are **immutable**.

👉 Once we create an object, we cannot change it.
👉 If we try to modify it, a **new object is created**.

### Why immutability?

Python checks:

* If an object already exists → reuse it
* Else → create a new object

### Advantages:

* Better memory utilization
* Improved performance

### Problem without immutability:

If multiple references point to the same object, modifying it affects all references.

👉 To prevent this, immutability is enforced.

### Example:

```
>>> a = 10
>>> b = 10

>>> a is b
>>> id(a)
>>> id(b)
```

---

## 🔹 bytes Data Type

Represents a group of byte numbers (like an array).

### ✅ Conclusion 1:

* Allowed values: **0 to 255**
* Otherwise → `ValueError`

### ✅ Conclusion 2:

* Bytes are **immutable**
* Cannot modify elements → `TypeError`

### Example:

```
>>> x = [10,20,30,40]
>>> b = bytes(x)

>>> b[0] = 100
```

---

## 🔹 bytearray Data Type

Same as `bytes`, but **mutable** (can be changed).

### Example 1:

```
x = [10,20,30,40]
b = bytearray(x)

for i in b:
    print(i)

10
20
30
40

b[0] = 100

for i in b:
    print(i)

100
20
30
40
```

### Example 2:

```
>>> x = [10,256]
```

---

