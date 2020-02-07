---
title: WindowAttach
---

# Attributes

| Name | Use |
| ----------------- | ------------------------------- ----------------------------- |
| IsDragElement | Whether to allow the current element to drag the form |
| IgnoreAltF4 | Whether to ignore the shortcuts Alt and F4 (the keyboard quickly exits or ends the currently running application) |
| ShowInTaskManager | Whether the form is displayed in the task manager |

# Use Cases

## IsDragElement Whether to allow the current element to drag the form

```xml
<hc:BlurWindow x:Class="Class namespace"
			 .....Regular item......
             WindowStartupLocation="CenterScreen"
             ShowTitle="True"
             Style="{DynamicResource WindowBlur}"
             xmlns:hc="https://ghost1372.github.io/handycontrol"
             d:DesignHeight="450" d:DesignWidth="800">
    <hc:SimplePanel>
        <Rectangle VerticalAlignment="Top" Margin="10" Height="30" RadiusX="4" RadiusY="4" Stroke="{DynamicResource BorderBrush}" StrokeDashArray="2,2"/>
        <Border hc:WindowAttach.IsDragElement="True" VerticalAlignment="Top" Margin="11" Height="28" Background="{DynamicResource DarkDefaultBrush}" CornerRadius="4">
            <TextBlock Text="DragHere" Style="{StaticResource TextBlockDefault}"/>
        </Border>
        <Button HorizontalAlignment="Right" Margin="0,15,15,0" VerticalAlignment="Top" Padding="0" Height="20" Width="20" Style="{StaticResource ButtonPrimary}" hc:IconElement.Geometry="{StaticResource CloseGeometry}" hc:BorderElement.CornerRadius="15"/>
    </hc:SimplePanel>
</hc:BlurWindow>
```

You can drag the form in the dark frame area

![WindowAttach.IsDragElement](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/attach/WindowAttach.IsDragElement.png)

## IgnoreAltF4 Whether to ignore the shortcut keys Alt and F4

Alt + F4 to close the window.

```xml
<Setter Property = "hc: WindowAttach.IgnoreAltF4" Value = "True" />
```

## ShowInTaskManager Whether to show the form to the task manager

Prerequisites:

-The window must be non-modal, that is, you cannot use `ShowDialog` to display the window.
-The window must also set `ShowInTaskBar` to` false`

ps: The effect of this additional property is not very obvious in `Windows7`