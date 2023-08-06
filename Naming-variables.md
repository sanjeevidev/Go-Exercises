# Go Variable Naming Rules

## Rules

- A variable name must start with a letter or an underscore character (`_`). Example: `_variable`, `variable`.
- A variable name cannot start with a digit. Example: `variable123` (incorrect).
- A variable name can only contain alpha-numeric characters and underscores (a-z, A-Z, 0-9, and `_`). Example: `variable_name_123`.
- Variable names are case-sensitive (`age`, `Age`, and `AGE` are three different variables).
- There is no limit on the length of the variable name. Example: `very_long_variable_name`.
- A variable name cannot contain spaces. Example: `variable name` (incorrect).
- The variable name cannot be any Go keywords. Example: `if`, `for`, `func` (incorrect).

## Multi-Word Variable Names

### Camel Case
Each word, except the first, starts with a capital letter:

```go
myVariableName = "John"
```

### Pascal Case
Each word starts with a capital letter:

```go
MyVariableName = "John"
```

### Snake Case
Each word is separated by an underscore character:

```go
my_variable_name = "John"
```
