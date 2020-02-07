---
title: DatePicker
---

# DatePickerBaseStyle

Native date picker default style, not recommended for direct use, should always be used by other styles in the BasedOn mode. The native date picker uses this style by default if no style is set:

- Default style
`<DatePicker SelectedDate="{x:Static system:DateTime.Now}"/>`
![ComboBoxBaseStyle](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/DatePickerBaseStyle.png)

# DatePickerExtendBaseStyle : DatePickerBaseStyle

The native date picker extends the default style and is not recommended for direct use. It should always be used by other styles in the BasedOn mode.

# DatePickerExtend : DatePickerExtendBaseStyle

- Heading on
`<DatePicker SelectedDate="{x:Static system:DateTime.Now}" Style="{StaticResource DatePickerExtend}" hc:InfoElement.Title="This is the title"/>`
![DatePickerExtend_1](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/DatePickerExtend_1.png)

- Heading left
`<DatePicker SelectedDate="{x:Static system:DateTime.Now}" Width="380" hc:InfoElement.TitleWidth="140" hc:InfoElement.TitleAlignment="Left" Style="{StaticResource DatePickerExtend}" hc:InfoElement.Title="Heading on the left"/>`
![DatePickerExtend_2](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/DatePickerExtend_2.png)

{% note warning %}
When the title is on the left, in order to align the left side of multiple input boxes, you need to set the title width. The title width does not need to be set one by one, and can be set uniformly on the external container.
{% endnote %}

- Heading on, with watermark
[See Combobox](https://handyorg.github.io/handycontrol/native_controls/comboBox/)

- Title is on, with watermark, and is required
[See Combobox](https://handyorg.github.io/handycontrol/native_controls/comboBox/)

- The title is on, with a watermark, and is required, and a custom required prompt
[See Combobox](https://handyorg.github.io/handycontrol/native_controls/comboBox/)