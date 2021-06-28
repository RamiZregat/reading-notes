# More CSS Layout
**- CSS Multi-column Layout:**
* The CSS multi-column layout allows easy definition of multiple columns of text - just like in newspapers: 
![](https://i.ibb.co/C8w0wSj/weq.png)

* CSS Multi-column Properties:
1. Column-count
2. Column-gap
3. Column-rule-style
4. Column-rule-width
5. Column-rule-color
6. Column-rule
7. Column-span
8. Column-width

* CSS Create Multiple Columns:
The `column-count` property specifies the number of columns an element should be divided into.  
The following example will divide the text in the `<div>` element into 3 columns:


```
<style>
.newspaper {
  column-count: 3;
}
</style>
```

* CSS Specify the Gap Between Columns: 
The `column-gap` property specifies the gap between the columns.
The following example specifies a 40 pixels gap between the columns:


```
<style>
.newspaper {
  column-count: 3;
  column-gap: 40px;
}
</style>
```

* CSS Column Rules: The `column-rule-style` property specifies the style of the rule between columns:



```
<style>
.newspaper {
  column-count: 3;
  column-gap: 40px;
  column-rule-style: solid;
}
</style>
```



* Specify How Many Columns an Element Should Span: The `column-span` property specifies how many columns an element should span across:




```
<style> 
.newspaper {
  column-count: 3;
  column-gap: 40px;
  column-rule: 1px solid lightblue;
}

h2 {
  column-span: all;
}
</style>
```



* Specify The Column Width: The `column-width` property specifies a suggested, optimal width for the columns.  
The following example specifies that the suggested, optimal width for the columns should be *100px*:



```
<style> 
.newspaper {
  column-width: 100px;
}
</style>
```

