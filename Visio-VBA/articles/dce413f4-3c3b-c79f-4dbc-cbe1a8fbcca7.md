
# Curve.End Property (Visio)

Returns the endpoint of a  **Curve** object. Read-only.


## Syntax

 _expression_ . **End**

 _expression_ A variable that represents a **Curve** object.


### Return Value

Double


## Remarks

The  **End** property of a **Curve** object returns the endpoint of a curve. A **Curve** object describes itself in terms of its parameter domain, which is the range [Start(),End()] where End() produces the curve's endpoint.


## Example

This Microsoft Visual Basic for Applications (VBA) macro shows how to use the  **End** property to determine the endpoint of a curve.


```vb
 
Sub End_Example() 
 
 Dim vsoShape As Visio.Shape 
 Dim vsoPaths As Visio.Paths 
 Dim vsoPath As Visio.Path 
 Dim vsoCurve As Visio.Curve 
 Dim dblStartpoint As Double 
 Dim dblEndpoint As Double 
 Dim intOuterLoopCounter As Integer 
 Dim intInnerLoopCounter As Integer 
 
 'Get the Paths collection for this shape. 
 Set vsoPaths = ActivePage.DrawOval(1, 1, 4, 4).Paths 
 
 'Iterate through the Path objects in the Paths collection. 
 For intOuterLoopCounter = 1 To vsoPaths.Count 
 Set vsoPath = vsoPaths.Item(intOuterLoopCounter) 
 Debug.Print "Path object " &amp; intOuterLoopCounter 
 
 'Iterate through the curves in a Path object. 
 For intInnerLoopCounter = 1 To vsoPath.Count 
 
 Set vsoCurve = vsoPath(intInnerLoopCounter) 
 Debug.Print "Curve number " &amp; intInnerLoopCounter 
 
 'Display the start point of the curve. 
 dblStartpoint = vsoCurve.Start 
 Debug.Print "Startpoint= " &amp; dblStartpoint 
 
 'Display the endpoint of the curve. 
 dblEndpoint = vsoCurve.End 
 Debug.Print "Endpoint= " &amp; dblEndpoint 
 
 Next intInnerLoopCounter 
 Debug.Print "This path has " &amp; intInnerLoopCounter - 1 &amp; " curve object(s)." 
 
 Next intOuterLoopCounter 
 Debug.Print "This shape has " &amp; intOuterLoopCounter - 1 &amp; " path object(s)." 
 
End Sub 

```

