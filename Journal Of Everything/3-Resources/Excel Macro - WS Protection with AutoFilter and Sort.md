#VBA #Excel
```vb
Private Sub Worksheet_SelectionChange(ByVal Target As Range)
    With Me.ListObjects(1) ' Assumes there is one and only one Table on the sheet. Modify as necessary
    If Target.Cells.CountLarge = 1 And Not Intersect(Target, .HeaderRowRange) Is Nothing Then
            Me.Unprotect
            .ShowAutoFilterDropDown = True ' Optional
    Else
            Me.Protect
            .ShowAutoFilterDropDown = False ' Optional
        End If
    End With
End Sub
```
