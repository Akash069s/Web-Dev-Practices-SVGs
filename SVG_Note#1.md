# Notes 1

## The SVG tag

The entire SVG needs a canvas to be drawn in. So an `<svg> </svg>` enclosing the entire content of svgs need to be intialised first.
After that you need to specify the ***height*** and ***width*** attributes of the SVG tag.

_An Important factor to note is that if the SVG overflows over the speculated boundry, the overflow won't be visible._

```
        The order in which you declare the elements will decide
        which element comes in front or the back.
        If I want the rectangle to be at the back of the circles then
        declare the rectangle first
```        
## Various shapes that can be used inside the `<svg>` block

- Circle

Attributes used:
1. r->radius
2. cx-> center_x
3. cy-> center_y
4. fill->background_color
5. stroke-> border
6. stroke-width -> border width

`<circle r="100" cx="125" cy="500" fill="none" stroke="black" stroke-width="10"/>`
`<circle r="70" cx="125" cy="300" fill="skyblue" stroke="black" stroke-width="10"/>`

- Rectangle

Attributes used:    
1. x->top_left
2. y->top_left
3. height,width -> self_explanatory
4. rx->rounded x axis (horizontal)
5. ry->rounded curve y axis (vertical)

`<rect rx="10" ry="10" x="275" y="75" height="100" width="100" fill="none" stroke="cyan" stroke-width="10"/>`    

- Line

Attributes used:
A line needs a starting and an ending point which is denoted by
1. x1->starting
2. y1->starting
**It is necessary to declare a stroke and stroke width for a line**

`<line x1="10" y1="125" x2="225" y2="225" stroke="none" stroke-width="25"/>`

- Polygon

Polygons need atleast 3 shapes to form, you can add points which will form 
the corners of the polygon.
`<polygon fill="crimson" points="50,50 125,125 200,50 200,200 125,125 50,200" />`


***You can either use `<shape_name /> or <shape_name></shape_name>`***