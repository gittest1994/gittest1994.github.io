---
title: TitleElement
---

# Attributes

| Name | Use |
| -------------- | ------------ |
| Title | Title Information |
| Background | Title Background Color |
| Foreground | Title Font Color |
| BorderBrush | Title Border Color |
| TitleAlignment | Title Alignment |
| TitleWidth | Title Width |

# Use Cases

## Title

```xml
     <hc:TextBox hc:TitleElement.Title="Title Information"
                 Margin="10,10"></hc:TextBox>
```

![TitleElement.Title](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/attach/TitleElement.Title.png)

## TitleAlignment

```xml
     <!--The title is on the top side -->
     <hc:TextBox hc:TitleElement.Title="Title Information"
              Hc:TitleElement.TitleAlignment="Top"
              Margin="10,10"></hc:TextBox>
     <!--The title is on the left -->
     <hc:TextBox hc:TitleElement.Title="Title Information"
              Hc:TitleElement.TitleAlignment="Left"
              Margin="10,10"></hc:TextBox>
```

![TitleElement.TitleAlignment](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/attach/TitleElement.TitleAlignment.png)

## TitleWidth

```xml
         <!--Set TitleWidth to Auto-->
         <hc:TextBox hc:TitleElement.Title="Title Information"
              Hc:TitleElement.TitleAlignment="Left"
              Hc:TitleElement.TitleWidth="Auto"
              Margin="10,10"></hc:TextBox>
         <!--Set TitleWidth to a specific value -->
         <hc:TextBox hc:TitleElement.Title="Title Information"
              Hc:TitleElement.TitleAlignment="Left"
              Hc:TitleElement.TitleWidth="60"
              Margin="10,10"></hc:TextBox>
```

![TitleElement.TitleWidth](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/attach/TitleElement.TitleWidth.png)