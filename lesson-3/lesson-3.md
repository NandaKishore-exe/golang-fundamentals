# Lesson 03 - Integer Data Types

## Topics Covered

- Signed integers (`int8`, `int16`, `int32`, `int64`)
- Unsigned integers (`uint8`, `uint16`, `uint32`, `uint64`)
- `int` and `uint`
- `byte` (alias for `uint8`)
- `rune` (alias for `int32`)
- Type casting between numeric data types

---

## Integer Types

### Signed Integers

| Type  | Size   | Range                                                   |
| ----- | ------ | ------------------------------------------------------- |
| int8  | 8-bit  | -128 to 127                                             |
| int16 | 16-bit | -32,768 to 32,767                                       |
| int32 | 32-bit | -2,147,483,648 to 2,147,483,647                         |
| int64 | 64-bit | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |

> Signed integers can store both positive and negative values.

---

### Unsigned Integers

| Type   | Size   | Range                           |
| ------ | ------ | ------------------------------- |
| uint8  | 8-bit  | 0 to 255                        |
| uint16 | 16-bit | 0 to 65,535                     |
| uint32 | 32-bit | 0 to 4,294,967,295              |
| uint64 | 64-bit | 0 to 18,446,744,073,709,551,615 |

> Unsigned integers store only positive values.

---

### Other Related Types

| Type | Description                                       |
| ---- | ------------------------------------------------- |
| byte | Alias for `uint8`                                 |
| rune | Alias for `int32` (stores Unicode code points)    |
| int  | 32-bit or 64-bit depending on system architecture |
| uint | 32-bit or 64-bit depending on system architecture |

---

## Type Casting

Go does **not** perform implicit type conversion.

```go
var a int8 = 10
var b int = int(a)
```

Convert using:

```go
type(value)
```

Examples:

```go
int(x)
float64(x)
uint(x)
string(x)
```

---

## Code Written

- Declared signed and unsigned integers.
- Used `byte` and `rune`.
- Practiced explicit type conversion.

---

## Key Notes

- Signed integers store both positive and negative values.
- Unsigned integers store only positive values.
- `byte` is an alias for `uint8`.
- `rune` is an alias for `int32`.
- `int` and `uint` size depends on the machine architecture (32-bit or 64-bit).
- Go requires explicit type conversion between different data types.
