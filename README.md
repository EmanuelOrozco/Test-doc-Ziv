# Data Types in Ziv Language

Below are the basic data types supported by this language, along with their usage and examples.

## Table of Contents

- [Type int](#type-int)
- [Type float](#type-float)
- [Type bool](#type-bool)
- [Type char](#type-char)
- [Type string](#type-string)
- [Type void](#type-void)
- [Type null](#type-null)
- [Summary Table](#summary-table)

## Type `int`

The `int` type (integer) is used to represent whole numbers, that is, numbers without decimals or fractions. This type is suitable for values like counts, loop indices, and mathematical operations without decimals.

- **Declaration and Assignment**:
```ziv
num1: int = 10
num2: int = 7
```

- **Usage Example**:

```ziv
// hello.ziv
fn main() {
  n: int = 10
  if (n > 5) {
  print("The number is higher")
  }
}
```

## Type `float`

The `float` type represents floating-point numbers, that is, numbers with decimals. This type is used for values that require decimal precision, such as measurements, scientific, and financial calculations.

- **Declaration and Assignment**:
```ziv
pi: float = 3.14159
temperature: float = 37.4
```

- **Usage Example**:
```ziv
// hello.ziv
fn main() {
  price: float = 19.99
  discount: float = price * 0.1 # Apply a 10% discount
}
```

## Type `bool`

The `bool` type (boolean) is used to represent logical values, that is, true or false. This type is essential for control flow operations and is used in conditional expressions. 

- **Declaration and Assignment**:
```ziv
is_adult: bool = True
is_active: bool = False
```

- **Usage Example**:
```ziv
// hello.ziv
fn main() {
  age: int = 30
  is_older: bool = age > 20
  if (is_older) {
    print("The number is higher")
  }
}
```

## Type `char`

The `char` type represents a single character, such as a letter, digit, or symbol. It is useful for handling text at the individual character level, such as text analysis or processing specific characters.

- **Declaration and Assignment**:
```ziv
initial: char = ‘A’
symbol: char = ‘#’
```

- **Usage Example**:
```ziv
// hello.ziv
fn main() {
  gender: char = ‘F’
  if (gender == ‘F’) {
    print(" Female gender")
  }
}
```

## Type `string`

The `string` type represents a sequence of characters or text. It is used to work with words, phrases, and any textual data.

- **Declaration and Assignment**:
```ziv
name: string = “John”
text: string = “Hello world!”
```

- **Usage Example**:
```ziv
// hello.ziv
fn main() {
  message: string = “Welcome to Ziv Language”
  print(message)
}
```

## Type `void`

The `void` type indicates the absence of a value. It is generally used to specify that a function does not return any value.

- **Function Declaration**:
```ziv
fn restore(item: string) -> void {
	print(item)
}
```

- **Usage Example**:
```ziv
restore(item: string) # Calls the function without expecting a return value
```	

## Type `null`

The `null` type represents the absence of value or a lack of a valid value. It is used to indicate that a variable does not contain data.

- **Declaration and Assignment**:
```ziv
name: string = null # The variable has no assigned value
```

- **Usage Example**:
```ziv
// hello.ziv
fn main() {
  name: string = null
  if (name == null){
    print(“Name not assigned”)
  }
}
```

## Summary Table

| Type     | Description                                   | Declaration Example              |
|----------|-----------------------------------------------|----------------------------------|
| `int`    | Integer number                                | `age: int = 30`                 |
| `float`  | Decimal number                                | `height: float = 1.75`          |
| `bool`   | Logical value (true/false)                    | `is_valid: bool = true`          |
| `char`   | Single character                              | `letter: char = 'A'`            |
| `string` | Text string                                   | `name: string = "John"`        |
| `void`   | No value (for functions)                      | `process() -> void {...}`   |
| `null`   | Absence of an assigned value                  | `text: string = null`           |
