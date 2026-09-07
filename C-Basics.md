# C Basics

## 1. Data Types

Data types tell us what kind of value a variable can store.

| Data Type | Description                                                      |
| --------- | ---------------------------------------------------------------- |
| `int`     | Used for storing whole numbers.                                  |
| `float`   | Used for storing decimal numbers.                                |
| `double`  | Used for storing decimal numbers with more precision than float. |
| `char`    | Used for storing a single character.                             |
| `bool`    | Used for storing true or false values.                           |
| `void`    | Used when there is no value.                                     |

## 2. Format Specifiers

Format specifiers are used with functions like `printf()` and `scanf()` to tell C what type of data is being used.

| Format Specifier | Used For                                  |
| ---------------- | ----------------------------------------- |
| `%d`             | Signed integer                            |
| `%u`             | Unsigned integer                          |
| `%o`             | Octal number                              |
| `%x`             | Hexadecimal number (lowercase)            |
| `%X`             | Hexadecimal number (uppercase)            |
| `%f`             | Floating-point number                     |
| `%e`             | Floating-point number in exponential form |
| `%c`             | Character                                 |
| `%s`             | String                                    |
| `%ld`            | Long integer                              |

## 3. Input/Output Functions

### scanf()

`scanf()` is used to take input from the user.

```c
scanf("%d", &num);
```

### printf()

`printf()` is used to display output on the screen.

```c
printf("%d", num);
```

### getchar()

`getchar()` is used to take one character as input.

```c
char ch;
ch = getchar();
```

### putchar()

`putchar()` is used to display one character.

```c
putchar(ch);
```

### fgets()

`fgets()` is used to take a string as input. It can also read spaces.

```c
fgets(name, sizeof(name), stdin);
```

### puts()

`puts()` is used to display a string.

```c
puts(name);
```

## 4. Escape Sequences

Escape sequences are used to perform special actions when writing characters inside a string.

| Escape Sequence | Meaning      | Example                   |
| --------------- | ------------ | ------------------------- |
| `\n`            | New line     | `printf("Hello\nWorld");` |
| `\t`            | Tab          | `printf("Name\tAge");`    |
| `\\`            | Backslash    | `printf("\\");`           |
| `\"`            | Double quote | `printf("\"Hello\"");`    |
| `\'`            | Single quote | `printf("\'A\'");`        |

## 5. Precision

Precision is used to control how many digits are shown after the decimal point when displaying a floating-point number.

It is written after a dot in the format specifier.

For example:

```c
printf("%.2f", 12.3456);
```

The output will be:

```text
12.35
```

Here, `.2` means that 2 digits will be displayed after the decimal point.

We can also use `.3`:

```c
printf("%.3f", 12.3456);
```

This gives:

```text
12.346
```
