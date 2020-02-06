
Markdown File Example
=====================

Contents
========



The library implements a method called ``new_table`` that can create tables using a list of strings. This method only needs: the number of rows and columns that your table must have. Optionally you can align the content of the table using the parameter ``text_align``

```python
list_of_strings = ["Items", "Descriptions", "Data"]
for x in range(5):
	list_of_strings.extend(["Item " + str(x), "Description Item " + str(x), str(x)])
mdFile.new_line()
mdFile.new_table(columns=3, rows=6, text=list_of_strings, text_align='center')
```  

|Items|Descriptions|Data|
| :---: | :---: | :---: |
|Item 0|Description Item 0|0|
|Item 1|Description Item 1|1|
|Item 2|Description Item 2|2|
|Item 3|Description Item 3|3|
|Item 4|Description Item 4|4|
