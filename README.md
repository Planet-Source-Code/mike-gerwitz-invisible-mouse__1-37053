<div align="center">

## Invisible Mouse


</div>

### Description

Squeak be gone! Have you ever wondered how to hide the user's cursor (mouse pointer)? Well, this simple API call will do the trick! See what you can do with it, and please vote!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Mike Gerwitz](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mike-gerwitz.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mike-gerwitz-invisible-mouse__1-37053/archive/master.zip)

### API Declarations

```
Public Declare Function ShowCursor Lib "user32" Alias "ShowCursor" (ByVal bShow As Long) As Long
```


### Source Code

```
Option Explicit
'This is the API function that will hide the cursor
Public Declare Function ShowCursor Lib "user32" Alias "ShowCursor" (ByVal bShow As Long) As Long
Private Sub Form_Load()
  'Hide the cursor when the program starts
  ShowCursor 0
End Sub
Private Sub Form_Unload()
  'Show the cursor when it ends
  ShowCursor 1
End Sub
```

