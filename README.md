# Compiler Design Assignment 1

- Upendra Kumar, IS201401048

Write regular definitions of the following languages:

1. All strings of lowercase letters that contain the five vowels in order.

```
    S -> T* a(T|a)* e(T|e)* i(T|i)* o(To)* u(T|u)*

    T -> [bcdfghjklmnpqrstvwxyz]
```

2. All strings of lowercase letters in which the letters are in ascending lexicographic order.

```
    a*b*c*d*e*f*g*h*i*j*k*l*m*n*o*p*q*r*s*t*u*v*w*x*y*z*
```
3. Comments, consisting of a string surrounded by `/*` and `*/`, without an intervening `*/` unless it is inside double quotes.
```
    \/\*(".*"|\*+[^/]|[^*"]*)*\*\/
    
    Here:
    ^ represents negation
    \/ represents /
    \* represents *
    . represents any character
    * represents 0 or more occurences
    + represents 1 or more occurences
    [] is used for set of characters
```
4. All strings of digits with no repeated digits.
5. All strings of digits with at most one repeated digit.
