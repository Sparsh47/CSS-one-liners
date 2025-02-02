1.

## Description

The css code allows you to combine the use of more than one css pseudo class.

### Long line of code

```
a:hover,
a:focus{
    color: #000000;
}
```

### One-liner

```
a:where(:hover, :focus){
    color: #000000;
}
```

---

2.

## Description

The css code allows you to set max-width and width on a container(or selector).

### Long line of code

```
.container {
    max-width: 900px;
    width: 70%;
}
```

### One-liner

```
.container {
    width: min(900px, 70%);
}
```

---

3.

## Description

This css code allows you to center items.

### Long line of code

```
.container {
    display: flex;
    justify-content: center;
    align-items: center;
}
```

### One-liner

```
.container {
    display: grid;
    place-items: center;
}
```

---

4.

## Description

This code is a shorthand for the four inset properties, top, right, bottom and left in one declaration.

### Long line of code

```
.card{
    position: fixed;
    top:0;
    right:0;
    bottom:0;
    left: 0;
}
```

### One-liner

```
.card{
    position: fixed;
    inset: 0;
}
```

---

5.

## Description

This code is a shorthand for applying same styling to multiple tags in one declaration.

### Long line of code

```
header p:hover{
    color:red;
    cursor:pointer;
}

main p:hover{
    color:red;
    cursor:pointer;
}

footer p:hover{
    color:red;
    cursor:pointer;
}
```

### One-liner

```
:is(header, main, footer) p:hover {
  color: red;
  cursor: pointer;
}
```

---

6.

The CSS :has selector helps you select elements that contain elements that match the selector you pass into the :has() function.

### Long line of code

```
h2,
.subtitle {
  margin: 0 0 1.5rem 0;
}
```

### One-liner

```
.header-group:has(h2):has(.subtitle) h2 {
  margin: 0 0 0.2rem 0;
}
```

---