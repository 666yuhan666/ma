# Table Multiline Backticks Test

## Test 1: Multiline backticks in cell
| Header 1 | Header 2 |
| -------- | -------- |
| `This is a
multiline
code block` | Cell 2 |
| Cell 3 | `Another
multiline
code block` |

## Test 2: Multiline backticks with pipes
| Header 1 | Header 2 |
| -------- | -------- |
| `Code | with
multiple
lines` | Cell 2 |

## Test 3: Table followed by code block
| Header 1 | Header 2 |
| -------- | -------- |
| `Multiline
code` | Cell 2 |
```
This should be a separate code block
Not part of the table
```

## Test 4: Code block followed by table
```
This is a code block
Before the table
```
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |

## Test 5: Incomplete table with multiline backticks
| Header 1 | Header 2 |
| -------- |
| `Multiline
code` | Cell 2 |
