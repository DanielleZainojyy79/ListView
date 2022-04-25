# ListView
$hListView = Eval("__hARC_ListView")     EndIf     $iColCount = _GUICtrlListView_GetColumnCount($hListView)     $aiGetSize = WinGetClientSize($hWnd)     $iWidth = Int($aiGetSize[0] / $iColCount)     For $i = 0 To $iColCount         _GUICtrlListView_SetColumnWidth($hListView, $i, $iWidth)     Next EndFunc   ;==>_GUICtrlListView_AutoResizeColumn
