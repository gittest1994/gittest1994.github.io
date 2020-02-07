---
title: DatePicker
---

The DatePicker control allows the user to select a date by typing the date in the text box or using the drop-down calendar control.

``` CS
[TemplatePart(Name = ElementTextBox, Type = typeof(DatePickerTextBox))]
public class DatePicker : System.Windows.Controls.DatePicker, IDataInput
```

# Create DatePicker

``` XML
<hc:DatePicker />
```

``` CS
var datePicker = new DatePicker();
```

The generated DatePicker is shown below:

![DatePicker](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/extend_controls/DatePicker_1.png)

# Select date

You can enter the date through the text box, or click the button to the right of the text box to open the drop-down calendar control to select the date.

![DatePicker](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/extend_controls/DatePicker_2.png)

You can also set the date like this in a XAML clock or code.

``` XML
<hc:DatePicker SelectedDate="{x:Static system:DateTime.Now}"/>
```

``` CS
datePicker.SelectedDate = DateTime.Now;
```
# Set title and placeholder text

You can add Headers and Placeholders to the DatePicker to indicate to the user what they do.

``` XML
<hc:DatePicker hc:InfoElement.TitleWidth="140"
               hc:InfoElement.TitleAlignment="Left"
               hc:InfoElement.Placeholder="{x:Static langs:Lang.PlsEnterContent}"
               hc:InfoElement.Title="{x:Static langs:Lang.TitleDemoStr3}" />
```
# Attributes

| Properties | Description |
| ---------------- | ------------------ |
| SelectedDate | Get or set the currently selected date |
| VerifyFunc | Get or Set Data Validation Delegation |
| IsError | Get or set whether the data is wrong |
| ErrorStr | Get or Set Error Alert |
| TextType | Get or Set Text Type |
| ShowClearButton | Gets or sets whether to show the clear button |

# Method

| Method | Description |
| ---------------- | ------------------ |
| VerifyData () | Verify Data |
