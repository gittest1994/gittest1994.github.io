---
title: PasswordBox
---

# PasswordBoxBaseStyle

The default style of the native password box is not recommended. It should always be used by other styles based on On.

{% note info no-icon %}
Example：
{% code %}
    <PasswordBox PasswordChar="*" VerticalAlignment="Center" Width="120"></PasswordBox>
{% endcode %}

![PasswordBox.BaseStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/PasswordBox.BaseStyle.png)

{% endnote %}

# PasswordBoxExtendBaseStyle : PasswordBoxBaseStyle

The native password box extends the default style. It is not recommended to use it directly, and it should always be used by other styles as BasedOn.

# PasswordBoxExtend : PasswordBoxExtendBaseStyle

Compared to the default style of the native password box, it can implement the functions of title and watermark with the help of additional attributes.

{% note info no-icon %}
用例：
{% code %}
    <!--In order to display the watermark in the normal password input text box, you need to set PasswordBoxAttach.PasswordLength="0"-->
    <PasswordBox Style="{DynamicResource PasswordBoxExtend}" PasswordChar="*" 
                 hc:PasswordBoxAttach.PasswordLength="0"
                 hc:InfoElement.Placeholder="Please enter the password" 
                 VerticalAlignment="Center"
                 Width="120"></PasswordBox>
    <PasswordBox Style="{DynamicResource PasswordBoxExtend}" PasswordChar="*" 
                 hc:TitleElement.Title="user password:"
                 hc:TitleElement.TitleAlignment="Top"
                 VerticalAlignment="Center"
                 Width="120"></PasswordBox>
{% endcode %}

![PasswordBox.ExtendStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/PasswordBox.ExtendStyle.png)

{% endnote %}