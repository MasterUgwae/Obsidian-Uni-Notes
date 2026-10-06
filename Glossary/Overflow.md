---
tags:
  - CS132
  - Glossary
---
## Definition
When completing an arithmetic operation and the word size is not large enough to represent all of the carry digits

## Example

|     | 1   | 0   | 0   | 1   | 1   | 0   | 0   |
| --- | --- | --- | --- | --- | --- | --- | --- |
| +   | 1   | 0   | 1   | 0   | 1   | 1   | 1   |
| 1   | 0   | 1   | 0   | 0   | 0   | 1   | 1   |
As the word length is 8 bits, the 9th bit that would be required to represent the final carry would overflow and often not be represented.