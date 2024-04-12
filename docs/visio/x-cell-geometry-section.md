---
title: "X Cell (Geometry Section)"
 
 
manager: lindalu
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm1135
 
ms.localizationpriority: medium
ms.assetid: 2416b323-e084-18e1-c9be-a797078dfab9

description: "Represents an x -coordinate on a shape in local coordinates. This table describes the X cell based on the row in which it's located."
---

# X Cell (Geometry Section)

Represents an  *x*  -coordinate on a shape in local coordinates. This table describes the X cell based on the row in which it's located.
  
|Row|Description|
|:-----|:-----|
|[MoveTo](moveto-row-geometry-section.md) <br/> | If the MoveTo row is the first row in the section, the X cell represents the *x* -coordinate of the first vertex of a path. If the MoveTo row appears between two rows, the X cell represents the *x* -coordinate of the first vertex after the break in the path. |
|[LineTo](lineto-row-geometry-section.md) <br/> | The *x* -coordinate of the ending vertex of a straight line segment. |
|[ArcTo](arcto-row-geometry-section.md) <br/> | The *x* -coordinate of the ending vertex of an arc. |
|[EllipticalArcTo](ellipticalarcto-row-geometry-section.md) <br/> | The *x* -coordinate of the ending vertex of an elliptical arc. |
|[PolylineTo](polylineto-row-geometry-section.md) <br/> | The *x* -coordinate of the ending vertex of a polyline. |
|[NURBSTo](nurbsto-row-geometry-section.md) <br/> | The *x* -coordinate of the last control point of a nonuniform rational B-spline (NURBS). |
|[SplineStart](splinestart-row-geometry-section.md) <br/> | The *x* -coordinate of a spline's second control point. |
|[SplineKnot](splineknot-row-geometry-section.md) <br/> | The *x* -coordinate of a control point. |
|[InfiniteLine](infiniteline-row-geometry-section.md) <br/> | An *x* -coordinate of a point on the infinite line. |
|[Ellipse](ellipse-row-geometry-section.md) <br/> | The *x* -coordinate of the center of the ellipse. |

## Remarks

To get a reference to the X cell by name from another formula, or from a program using the **CellsU** property, use:
  
||Value |
|:-----|:-----|
| **Cell name:**  <br/> | Geometry *i* .X  *j*            where  *i*  and  *j*  = <1>, 2, 3... |
| **Cell name:**  <br/> | Geometry *i* .X1 (InfiniteLine and Ellipse rows)            where  *i*  = <1>, 2, 3... |

To get a reference to the X cell by index from a program, use the **CellsSRC** property with the following arguments:
  
||Value |
|:-----|:-----|
| **Section index:**  <br/> |**visSectionFirstComponent** + *i*           where *i* = 0, 1, 2... |
| **Row index:**  <br/> |**visRowVertex** + *j*           where *j* = 0, 1, 2... |
| **Row index:**  <br/> |**visRowVertex** (InfiniteLine and Ellipse rows)  <br/> |
| **Cell index:**  <br/> |**visX** (MoveTo, LineTo, ArcTo, EllipticalArcTo, NURBSTo, Polyline, SplineStart, and SplineKnot rows)  <br/> |
| **Cell index:**  <br/> |**visInfiniteLineX1** (InfiniteLine row)  <br/> |
| **Cell index:**  <br/> |**visEllipseCenterX** (Ellipse row)  <br/> |
