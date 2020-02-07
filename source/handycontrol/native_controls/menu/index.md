---
title: Menu
---

# MenuBaseStyle

The default style of the menu is not recommended. It should always be used by other styles in the manner of BasedOn.

{% note info no-icon %}
用例：
{% code %}
    <Menu ItemsSource="{Binding Menus}">
        <Menu.ItemTemplate>
            <HierarchicalDataTemplate ItemsSource="{Binding Children}">
                <TextBlock Text="{Binding Name}"></TextBlock>
            </HierarchicalDataTemplate>
        </Menu.ItemTemplate>
</Menu>
{% endcode %}

![Menu.BaseStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/Menu.BaseStyle.png)

{% endnote %}