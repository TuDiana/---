# ---
计算机网络技术、Visual Basic 
VB循环结构
Private Sub Command1_Click()
n = 0
For i = 100 To 999
a = i \ 100
b = i \ 10 Mod 10
c = i Mod 10
If (c + b) Mod 10 = a Then
    x = 0
    For j = 2 To i - 1
        If i Mod j = 0 Then x = 1: Exit For
    Next j
    If x = 0 Then n = n + 1
End If
Next i
Print n
End Sub

Private Sub Form_Load()

End Sub
