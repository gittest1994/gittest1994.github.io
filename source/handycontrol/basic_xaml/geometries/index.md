---
title: Geometric shape
---

HandyControl comes with some geometric shape definitions, but it is obviously not enough to apply to production. We are not prepared to be all-encompassing. There is never a bottom, so we will do the opposite. It only contains the control library itself (of course users can also use it), and the rest should expand on its own. All shape definitions in the control library are listed in the following table:

| Name | Description |
|-|-|
| CalendarGeometry | Calendar |
| DeleteGeometry | Delete |
| DeleteFillCircleGeometry | Delete (Circular Fill) |
| CloseGeometry | Close |
| DownGeometry | Next |
| UpGeometry | On |
| ClockGeometry | Clock |
| LeftGeometry | Left |
| RightGeometry | Right |
| RotateLeftGeometry | Rotate Left |
| EnlargeGeometry | Zoom |
| ReduceGeometry | Zoom out |
| DownloadGeometry | Download |
| SaveGeometry | Save |
| WindowsGeometry | Window |
| FullScreenGeometry | Full Screen |
| FullScreenReturnGeometry | Full Screen Back |
| SearchGeometry | Search |
| UpDownGeometry | Upper and lower combinations |
| WindowMinGeometry | Window Minimization |
| WindowRestoreGeometry | Window Restore |
| WindowMaxGeometry | Window Maximization |
| AudioGeometry | Sound |
| BubbleTailGeometry | Bubble Tail |
| StarGeometry | Love |
| AddGeometry | Add |
| SubGeometry | Subtract |
| WarningGeometry | Warning |
| InfoGeometry | Information |
| ErrorGeometry | Error |
| SuccessGeometry | Success |
| FatalGeometry | Critical |
| AskGeometry | Inquiry |
| AllGeometry | All |
| DragGeometry | Drag and Drop (for toolbars) |
| CheckedGeometry | Checkbox Checked |
| EyeOpenGeometry | PasswordBox Show Password |
| EyeCloseGeometry | PasswordBox Hide Password |
| DropperGeometry | Select Color from Shell |
| VisualStudioGeometry | Visual Studio Icon |

{% note info no-icon %}
Example: `Data="{StaticResource DragGeometry}"`
{% endnote %}