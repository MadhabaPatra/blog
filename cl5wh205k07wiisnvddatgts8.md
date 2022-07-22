## Brief about CSS position

CSS permits various strategies for situating components. The most well-known are position, float, and display. Here, we'll make sense of how you can utilize the CSS position property to alter the design of your page. We'll investigate different position types and survey how you can situate components like text and images to make a delightful page plan.

## What Is Position in CSS?


- **CSS position** property is used to specify how the element will be displayed on the page. 
- The top, right, bottom, and left CSS position properties determine the final location of the element. However, these properties will not work unless the position property is set. They also work differently depending on the position value.

There are five types of positioning


1. Static Positioning
2. Relative Positioning
3. Fixed Positioning
4. Absolute Positioning
5. Sticky Positioning

#### 1.Static Positioning
- Static positioning is the default for every HTML element.
- Static positioned elements are not affected by the **top**, **bottom**, **left**, and **right **properties.
- For example: 
```
.static {
      position: static;
      border: 3px solid green;
      color: red;
    }
```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658491730669/Snn9HuGYm.png align="left")

#### 2.Relative Positioning
- **Relative positioned** element follows the render flow but will be shifted relative to its initial position.
- Setting the **top**, **right**, **bottom**, and **left **properties of a relatively-positioned element will cause it to be adjusted away from its normal position.
- For example: 
```
.relative {
      position: relative;
      left: 50px;
      border: 3px solid green;
      color: red;
    }
```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658492198399/uud6Kr32l.png align="left")


#### 3.Fixed Positioning
- **Fixed positioned** element is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled.
- The **top**, **right**, **bottom**, and **left **properties are used to position the element.
- For example: 
```
 .fixed {
      position: fixed;
      top: 20px;
      right: 0;
      border: 3px solid green;
      color: red;
    }
```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658492326837/BMm0zn9zG.png align="left")

#### 4.Absolute Positioning
- **Absolute positioned** element is positioned relative to the nearest positioned ancestor.
- The **top**, **right**, **bottom**, and **left **properties are used to position the element.
- Absolute positioned elements are removed from the normal flow, and can overlap elements.
- For example: 
```
.relative {
      position: relative;
      width: 400px;
      height: 200px;
      border: 3px solid red;
    }

    .absolute {
      position: absolute;
      top: 80px;
      right: 0;
      width: 200px;
      height: 100px;
      border: 3px solid green;
    }
```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658492722197/BlkzIi4BC.png align="left")

#### 5.Sticky Positioning
- **Sticky positioned** is positioned based on the user's scroll position.
- The **top**, **right**, **bottom**, and **left **properties are used to position the element.
- It toggles between **relative **and **fixed**, depending on the scroll position. It is positioned **relative **until a given offset position is met in the viewport - then it "sticks" in place
- For example: 
```
 .sticky {
      position: sticky;
      top: 0;
      background-color: green;
      border: 2px solid red;
    }
```

![Document - Google Chrome 2022-07-22 18-17-44_Trim.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1658494251567/30EVkdqal.gif align="left")

### Cheat sheet

For quick reference, here’s a cheat sheet for what we’ve learned.

**1.Position: static**


- Default positioning for all elements.
- Puts element in normal flow.


**2.Position: relative**


- Can be offset with top, right, bottom and left.
- Offset relative to itself.
- Creates relative-type positioning context for children.


 **3.Position: absolute**

- Can be offset with top, right, bottom and left.
- Offset relative to its nearest relative-type positioned parent.
- Creates relative-type positioning context for children.


 **4.Position: fixed**

- Can be offset with top, right, bottom and left.
- Offset relative to the viewport.
- Creates relative-type positioning context for children.

### References

[MDN docs](https://developer.mozilla.org/en-US/docs/Web/CSS/position)

[W3Schools docs](https://www.w3schools.com/css/css_positioning.asp)

[More details about CSS positions ](https://blog.hubspot.com/website/css-position)

### Finished
That's it for today!

Hope you liked the post, if you’ve got any questions your can Mail me madhabapatra@gmail.com.

Thanks