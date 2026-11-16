---
context: Food Ingredient
---


```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" 
WHERE contains(file.outlinks, this.file.link)
sort desc
```