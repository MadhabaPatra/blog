## What are CSS Selectors & How Do They Work?

## What are CSS selectors?

**CSS selectors** are used to define the elements you want to style with CSS. 
They can be broadly divided into six categories:

1. Universal Selector (*)
2. Individual selector (tag name)
3. Class (.) and Id (#) selector
4. Group Selector (,)
5. Combined selector (⎵ >  +  ~)
6. Pseudo selector (: or ::)





### 1.Universal Selector
- The universal selector (*) selects all HTML elements on the page.
- For example:

```
* {
  margin: 0;
  padding: 0;
  outline: 0;
  background-color: red;
}
/* Above CSS rule will affect every HTML element on the webpage*/``` 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658473767967/zHR3O6IWa.png align="left")

### 2.Individual selector
- The individual selector selects  HTML elements based on the element name.
- For example:

```
p {
  text-align: center;
  color: blue;
}
/* It target all <p> elements on the page.*/```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658473881408/7eMQXaXNQ.png align="left")
### 3.Class and Id selector

#### Id selector

- The id selector (#) selects a HTML element based on id of the element.
- To select a element based on id, use a hash (#) followed by the id of the element.
- For example

```
#top-modal {
      top: 0;
      left: 50%;
      padding: 25px;
      background-color: aqua;
      position: absolute;
    }
/* It target the element with the id (top-modal). */```


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658487779755/5_DqdM82C.png align="left")

#### Class selector

- The class selector (.) selects  HTML elements based on class name.
- To select all elements based on class name, use a hash (.) followed by the class of the elements.
- For example:

```
.text-danger {
  color: red;
}
/* It target the all elements with the class(text-danger). */```


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658487949739/zMVOne2mT.png align="left")


### 4.Group Selector
- Grouping selectors helps to select all elements that you want to give same css.
- To select all elements, you need to use a comma (,) to separate each element selector while grouping.
- For example:

```
.text-danger,
#text-alert,
span,
p {
  color: red;
}
/* It target the
all elements with the class (text-danger), 
element with id (text-alert), 
all <span> and <p> elements. 
*/```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658488146267/IxR0PJ0KO.png align="left")

### 5.Combined selector
- Combined selector explains the relationship between the selectors.
- A CSS selector can contain more than one  selector. Between the selectors, we can include a combined selector.

There are four different combined selectors in CSS:
#### 1. Descendant Selector (⎵)

- It matches all elements that are descendants of a specified element.
- The selectors are separated by the space (⎵).
- It combines more than one selectors whereas the first selector act as parent and second act as child for the first selector and the third selector act as child for second selector and so on.

- For example:

```
div span
{
  font-weight: 700;
  color:red;
}

/* It target 
all <span> elements 
which are child of hero class elements. 
*/```


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658489154697/KQuJCxjnV.png align="left")
#### 2. Child Selector (>)

- It matches all elements that are the direct children of a a specified element.
- The selectors are separated by the greater than sign(>).

- For example:

```
 div > span {
      color: red;
    }

/* It target all <span> elements that are direct children of a <div> element */```


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658488587021/aLVpTAyXf.png align="left")

#### 3. Adjacent Sibling Selector (+)

- It matches one elements that are the direct children and after the specified element.
- The selectors are separated by the plus sign(+).

- For example:

```
div + span
{
  color:red;
  text-align:center;
}
/* 
It target an <span> element that are neighbor to specified element just after the <div> element 
*/```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658488945408/i0DwxdMIJ.png align="left")

#### 4. General Sibling Selector (~)

- It matches all elements that are next siblings of a specified element.
- The selectors are separated by the tilde sign(~).

- For example:

```
div ~ span
{
  color:red;
  text-align:center;
}
/* It target all <p> elements that are next siblings of <div> elements. */```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658488971287/gGBdbzlfD.png align="left")
### 6.Pseudo selector
There are two type of Pseudo selector
#### 1. Pseudo-element Selector
- Pseudo-element selector is used to style specific parts/portions of specified elements.
- The pseudo-element selector is separated by double-colon (::).
- It can be used to style the first letter, or line, insert content before, or after, the content of an element.
- For example:

```
p::first-line
{
  font-weight:bold;
  color:aqua;
}
/* It target the first line of every <p> elements.  */```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658489240993/51eNQMgY2.png align="left")

For more information about Pseudo-element Selector, visit [here](https://www.w3schools.com/css/css_pseudo_elements.asp).

#### 2. Pseudo-classes Selector
- Pseudo-class selector is used to define a special state of an element.
- The pseudo-class selector is separated by double-colon (:).
- It can be used to style an element when a user hovers the mouse over it,when it gets focus and many more.
- For example:

```
a:hover
{
  color: red;
}
/* It styles <a> elements when someone hover mouse over it.  */```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658489369053/-opHNQQsW.png align="left")

For more information about Pseudo-classes Selector, visit [here](https://www.w3schools.com/css/css_pseudo_classes.asp).

### Finished
That's it for today!

Hope you liked the post, if you’ve got any questions your can Mail me madhabapatra@gmail.com.

Thanks
