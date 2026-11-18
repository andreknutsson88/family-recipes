---
context: Knowledge Category
---
[[00 Home 🌎]]
[[Knowledge MOC 🧠]]
[[AI recipe template]]


# Beef  🥩

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian"
FROM #recipe AND #beef WHERE file.name != "Template, Recepie"
sort desc
```

# Pork 🐷

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian" 
FROM #recipe AND #pork WHERE file.name != "Template, Recepie"
sort ASC
```

# Chicken 🍗

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian" 
FROM #recipe AND #kyckling WHERE file.name != "Template, Recepie"
sort desc
```

# Vegan and Vegetarian 🥗

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian" 
FROM #recipe AND #vegan  OR #vegetarian WHERE file.name != "Template, Recepie"
sort desc
```

# Pasta 🍝

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian" 
FROM #recipe AND #pasta  WHERE file.name != "Template, Recepie"
sort desc
```

# Fika ☕🍩🍪

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian"
FROM #recipe AND #fika WHERE file.name != "Template, Recepie"
sort desc
```

# Bread 🍞

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian" 
FROM #recipe AND #bread WHERE file.name != "Template, Recepie"
sort desc
```

# Sauce 🍲

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici", Rating_Julian AS "Julian" 
FROM #recipe AND #sauce WHERE file.name != "Template, Recepie"
sort desc
```

# [[Beverage ☕]]


# Other Recepies 🍽️

```dataview
TABLE WITHOUT ID file.link AS "Recepies" , cooking_time AS "Time [h]" , Rating_André AS "André", Rating_Meici AS "Meici" 
FROM #recipe WHERE file.name != "Template, Recipe"
WHERE !contains(tags, "vegan") 
AND !contains(tags, "pasta") 
AND !contains(tags, "kyckling")
AND !contains(tags, "fika")
AND !contains(tags, "beef")
AND !contains(tags, "bread")
AND !contains(tags, "pork")
AND !contains(tags, "vegetarian")
AND !contains(tags, "beverage")
AND !contains(tags, "sauce")
AND !contains(tags, "drink")
sort desc
```

# Ingredients
[[Cooking Ingredients]]

# Cooking related notes

```dataview
TABLE
FROM "Cards" 
WHERE contains(context, "Cooking") 
```

# Related
[[Knowledge MOC 🧠]]

