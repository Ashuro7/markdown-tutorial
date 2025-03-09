# Markdown-Tutorial

Headings start with a "#", the more number of hashes the smaller the font size of the heading. (Upto 6 "#")

## Lists

A list can be created simply by having a dash "-" and then a space, before the line/item.
- Item 1
- Item 2

## Bold, Italitcs, Strikethrough, Highlights
- *Italics* : This can be done by enclosing the string with single asterisks.
- **Bold** : The string should be wrapped around two asterisks.
- ~~Thermodynamics~~ : The string should be wrapped around two tildes (~) on both sides.
- <mark>Aerodynamics</mark> : Highlighting the text cannot be done in standard or github markdown style/flavor but can be acheived using the "mark" html tag.

## Superscripts and Subscripts
- superscript<sup>2</sup> : Cannot be done in standard or github markdown but can be achieved using the "sup" HTML tag.
- subscript<sub>2</sub> : Cannot be done in standard or github markdown but can be achieved using the "sub" HTML tag.

## Checklist
- [ ] An unchecked item in the checklist. It starts with a "-" then a space, then square brackets with space between them. This is unchecked.
- [x] A checked item in the checklist. It starts with a "-" then a space, then square brackets with an "x/X" between them.

## Quote Blocks
> Quote blocks are achieved by having a ">" before the line.

## Code Blocks
We can have "code" blocks by enclosing the code in backticks (``).
Multi-line code will be enclosed in three backticks (``````)

```py
def fact(n: int) -> int:
    if n == 1:
        return 1
    else:
        return n * fact(n-1)
```
Syntax highlighting can be done by specifiying the language after the first of the backticks pair as shown above. (py = python)

## Links

- [Google](https://www.google.com): Links can be displayed by having the overlayed text in square brackets followed by the link in parenthesis
- <https://www.google.com>: Links without an associated text can also be displayed as is or enclosed in tags <>

## Line Breaks
Lines can be displayed by having at least three dashes "---"

---

As shown, "---" gets you a line like above

## Tables

Columns are separated by a pipe "|". The column headers and the data rows is separated by three dashes "---". Dashes aren't required to separate each individual "data rows". Colons ":" to either or both side of the three dashes define the alignment (Left, Right, Centre)

| Name | Age | Email |
|----:|:----|:---|
|Ash | 20  | as@gmai.com|
|Gilgamesh| 19  | gil@gmail.com|
