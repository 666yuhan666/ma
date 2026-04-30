# Comprehensive Table Test

## Test 1: Table followed by code block
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
```
Code block after table
Should not be part of the table
```

## Test 2: Code block followed by table
```
Code block before table
Should not be part of the table
```
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |

## Test 3: Cell with escaped pipe
| Header 1 | Header 2 |
| -------- | -------- |
| Cell \| with pipe | Cell 2 |
| Cell 3 | Cell \| another pipe |

## Test 4: Cell with backticks and escaped pipe
| Header 1 | Header 2 |
| -------- | -------- |
| `Code \| with pipe` | Cell 2 |
| Cell 3 | `More \| code` |

## Test 5: Multiline backticks in cell
| Header 1 | Header 2 |
| -------- | -------- |
| `Multiline
code block` | Cell 2 |
| Cell 3 | `Another
multiline
code block` |

## Test 6: Incomplete table (missing delimiter row)
| Header 1 | Header 2 |
Cell 1 | Cell 2 |
Cell 3 | Cell 4 |

## Test 7: Incomplete table (mismatched columns)
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
| Cell 3 | Cell 4 | Cell 5 |

## Test 8: Table with complex content
| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| `Code \| with \| multiple \| pipes` | Cell 2 | `Another \| code` |
| Cell 4 | `Multiline
code \| with pipe` | Cell 6 |
