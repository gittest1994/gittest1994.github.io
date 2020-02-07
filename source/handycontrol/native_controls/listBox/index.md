---
title: ListBox
---

# ListBoxBaseStyle

  ListBox default style is not recommended to use directly, it should always be used by other styles in BasedOn mode.

{% note info no-icon %}
Example：
{% code %}
     <Style BasedOn = "{StaticResource ListBoxBaseStyle}" TargetType = "ListBox" />
{% endcode %}

![ListBox.BaseStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ListBox.BaseStyle.png)

{% endnote %}

#  ListBoxCustom : ListBoxBaseStyle

ListBox List Custom style, which retains the basic attribute style of the Listbox, and the data display style is customized by the current user to achieve personalized customization.

{% note info no-icon %}
Example：
{% code %}
    <ListBox Margin="10" ItemsSource="{Binding Datas}"  
             Style="{DynamicResource ListBoxCustom}">
        <ListBox.ItemTemplate>
            <DataTemplate>
                <Border BorderThickness="1" BorderBrush="Black" Margin="0,5">
                    <DockPanel LastChildFill="True">
                        <Path DockPanel.Dock="Left" Fill="YellowGreen" Width="20" Margin="10,0,10,0" HorizontalAlignment="Center" Data="{DynamicResource BubbleTailGeometry}"></Path>
                        <TextBlock Padding="10" Text="{Binding Name}"></TextBlock>
                    </DockPanel>
                </Border>
            </DataTemplate>
        </ListBox.ItemTemplate>
    </ListBox>
{% endcode %}



![ListBox.CustomStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ListBox.CustomStyle.png)

{% endnote %}

#  WrapPanelHorizontalListBox : ListBoxCustom

The layout container is WrapPanel, and the display style is horizontal.

{% note info no-icon %}
Example：
{% code %}
    <ListBox Margin="10" ItemsSource="{Binding Datas}"  
             Style="{DynamicResource WrapPanelHorizontalListBox}">
        <ListBox.ItemTemplate>
            <DataTemplate>
                <Border BorderThickness="1" BorderBrush="Black" Margin="5,0">
                    <DockPanel LastChildFill="True">
                        <Path DockPanel.Dock="Left" Fill="YellowGreen" Width="20" Margin="10,0,10,0" HorizontalAlignment="Center" Data="{DynamicResource BubbleTailGeometry}"></Path>
                        <TextBlock Padding="10" Text="{Binding Name}"></TextBlock>
                    </DockPanel>
                </Border>
            </DataTemplate>
        </ListBox.ItemTemplate>
    </ListBox>
{% endcode %}

![ListBox.WrapPanelHorizontalStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ListBox.WrapPanelHorizontalStyle.png)

{% endnote %}

#  WrapPanelVerticalListBox : ListBoxCustom

The layout container is WrapPanel, and the display style is vertical.

{% note info no-icon %}
Example：
{% code %}
    <ListBox Margin="10" ItemsSource="{Binding Datas}"  
             Style="{DynamicResource WrapPanelVerticalListBox}">
        <ListBox.ItemTemplate>
            <DataTemplate>
                <Border BorderThickness="1" BorderBrush="Black" Margin="0,5">
                    <DockPanel LastChildFill="True">
                        <Path DockPanel.Dock="Left" Fill="YellowGreen" Width="20" Margin="10,0,10,0" HorizontalAlignment="Center" Data="{DynamicResource BubbleTailGeometry}"></Path>
                        <TextBlock Padding="10" Text="{Binding Name}"></TextBlock>
                    </DockPanel>
                </Border>
            </DataTemplate>
        </ListBox.ItemTemplate>
    </ListBox>
{% endcode %}

![ListBox.WrapPanelVerticalStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ListBox.WrapPanelVerticalStyle.png)

{% endnote %}

#  StackPanelHorizontalListBox : ListBoxCustom

The layout container is a StackPanel, and the display style is horizontal.

{% note info no-icon %}
Example：
{% code %}
    <ListBox Margin="10" ItemsSource="{Binding Datas}"  
             Style="{DynamicResource StackPanelHorizontalListBox}">
        <ListBox.ItemTemplate>
            <DataTemplate>
                <Border BorderThickness="1" BorderBrush="Black" Margin="5,0">
                    <DockPanel LastChildFill="True">
                        <Path DockPanel.Dock="Left" Fill="YellowGreen" Width="20" Margin="10,0,10,0" HorizontalAlignment="Center" Data="{DynamicResource BubbleTailGeometry}"></Path>
                        <TextBlock Padding="10" Text="{Binding Name}"></TextBlock>
                    </DockPanel>
                </Border>
            </DataTemplate>
        </ListBox.ItemTemplate>
    </ListBox>
{% endcode %}

![ListBox.StackPanelHorizontalStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ListBox.StackPanelHorizontalStyle.png)

{% endnote %}

#  StackPanelVerticalListBox : ListBoxCustom

The layout container is a StackPanel, which displays the style vertically.

{% note info no-icon %}
Example：
{% code %}
    <ListBox Margin="10" ItemsSource="{Binding Datas}"  
             Style="{DynamicResource StackPanelVerticalListBox}">
        <ListBox.ItemTemplate>
            <DataTemplate>
                <Border BorderThickness="1" BorderBrush="Black" Margin="0,1">
                    <DockPanel LastChildFill="True">
                        <Path DockPanel.Dock="Left" Fill="YellowGreen" Width="20" Margin="10,0,10,0" HorizontalAlignment="Center" Data="{DynamicResource BubbleTailGeometry}"></Path>
                        <TextBlock Padding="10" Text="{Binding Name}"></TextBlock>
                    </DockPanel>
                </Border>
            </DataTemplate>
        </ListBox.ItemTemplate>
    </ListBox>
{% endcode %}

![ListBox.StackPanelVerticalStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ListBox.StackPanelVerticalStyle.png)

{% endnote %}