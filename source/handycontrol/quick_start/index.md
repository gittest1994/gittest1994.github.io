---
title: Quick start
---

# Easy Ways
Download the source code or reference the control library in Nuget mode or use Extension
Source link: [HandyControl-Github](https://github.com/HandyOrg/HandyControl)
Nuget link: [HandyControl-Nuget](https://www.nuget.org/packages/HandyControl/)
Extension link [HandyControl-Extension](https://marketplace.visualstudio.com/items?itemName=HandyOrg.handycontrolforvs2019)

{% note info %}

There is a Custom Version Called HandyControls

Source link: [HandyControls-Github](https://github.com/ghost1372/HandyControls)
Nuget link (Custom Version): [HandyControls-Nuget](https://www.nuget.org/packages/HandyControls)
Extension link (Custom Version) [HandyControls-Extension](https://marketplace.visualstudio.com/items?itemName=MahdiHosseini.HandyControls)

{% endnote %}

# Nuget

{% note warning %}
If you use custom version you don't need to add the following codes
{% endnote %}

Add the following code to App.xaml:

``` xml
<Application.Resources>
    <ResourceDictionary>
        <ResourceDictionary.MergedDictionaries>
            <ResourceDictionary Source="pack://application:,,,/HandyControl;component/Themes/SkinDefault.xaml"/>
            <ResourceDictionary Source="pack://application:,,,/HandyControl;component/Themes/Theme.xaml"/>
        </ResourceDictionary.MergedDictionaries>
    </ResourceDictionary>
</Application.Resources>
```

# Last step
Add a namespace: `xmlns:hc="https://handyorg.github.io/handycontrol"`

# Extension

just download and install handycontrol template from marketplace. in this way you dont need to add anything after installing hc, create new project with handycontrol template

![Extension](https://raw.githubusercontent.com/ghost1372/HandyControls/develop/Resources/vsixTemplate.png)