
# ShapeRange.Line Property (Excel)

Returns a  **[LineFormat](13eca34b-adf7-ddd3-8c73-cc8b508c624a.md)** object that contains line formatting properties for the specified shape. (For a line, the **LineFormat** object represents the line itself; for a shape with a border, the **LineFormat** object represents the border). Read-only.


## Syntax

 _expression_ . **Line**

 _expression_ A variable that represents a **ShapeRange** object.


## Example

This example adds a blue dashed line to  `myDocument`.


```vb
Set myDocument = Worksheets(1) 
With myDocument.Shapes.AddLine(10, 10, 250, 250).Line 
 .DashStyle = msoLineDashDotDot 
 .ForeColor.RGB = RGB(50, 0, 128) 
End With
```

This example adds a cross to  `myDocument` and then sets its border to be 8 points thick and red.




```vb
Set myDocument = Worksheets(1) 
With myDocument.Shapes.AddShape(msoShapeCross, 10, 10, 50, 70).Line 
 .Weight = 8 
 .ForeColor.RGB = RGB(255, 0, 0) 
End With
```


## See also


#### Concepts


[ShapeRange Object](e1b8229c-73a0-4a77-5e00-4bcec9032260.md)
