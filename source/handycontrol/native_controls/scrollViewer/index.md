---
title: ScrollViewer
---

# ScrollViewerNativeBaseStyle

The default style of the native scroll view is not recommended. It should always be used by other styles based on On.

Case:

```xml
<ScrollViewer>
   <Grid Height="500">
      <TextBlock Text="Content area"></TextBlock>
   </Grid>
</ScrollViewer>
```

effect:

![ScrollViewer.DefaultStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ScrollViewer.DefaultStyle.png)

# ScrollViewerUpDown

Scroll view style showing up and down buttons

Case:

```xml
<ScrollViewer Style="{StaticResource ScrollViewerUpDown}">
    <StackPanel Height="500">
        <TextBlock Text="Content area" Height="250"></TextBlock>
        <TextBlock Text="Content area" Height="250"></TextBlock>
        <TextBlock Text="Content area"></TextBlock>
        <TextBlock Text="Content area"></TextBlock>
    </StackPanel>
</ScrollViewer>
```

effect:

![ScrollViewer.UpDownStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ScrollViewer.UpDownStyle.png)
