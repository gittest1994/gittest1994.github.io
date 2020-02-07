---
title: ProgressBar
---

# ProgressBarBaseStyle

The default style of the progress bar. It is not recommended to use it directly, and it should always be used by other styles as BasedOn.

# Other styles

Other styles and effects included in `HandyControl`, including the following styles:

| Style Key | Uses | Parent Style |
| ------------------ | ---- ||
| ProgressBarSuccess | Progress bar progress bar | ProgressBarBaseStyle |
| ProgressBarInfo | Prompt Color Progress Bar | ProgressBarBaseStyle |
| ProgressBarWarning | Warning color progress bar | ProgressBarBaseStyle |
| ProgressBarDanger | Dangerous Progress Bar | ProgressBarBaseStyle |
| ProgressBarStripeBaseStyle | Stripe progress bar default style (not recommended for direct use) |-|
| ProgressBarPrimaryStripe | Stripe Progress Bar | ProgressBarStripeBaseStyle |
| ProgressBarSuccessStripe | Progress Bar Stripe Progress Bar | ProgressBarStripeBaseStyle |
| ProgressBarInfoStripe | Information color stripe progress bar | ProgressBarStripeBaseStyle |
| ProgressBarWarningStripe | Progress bar with warning stripes | ProgressBarStripeBaseStyle |
| ProgressBarDangerStripe | Dangerous Stripe Progress Bar | ProgressBarStripeBaseStyle |
| ProgressBarFlat | Flat style |-|

Case:

```xml
<StackPanel Margin="20">
        <TextBlock Text="Default style"></TextBlock>
        <ProgressBar Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarSuccess"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarSuccess}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarInfo"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarInfo}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarWarning"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarWarning}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarDanger"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarDanger}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarPrimaryStripe"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarPrimaryStripe}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarSuccessStripe"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarSuccessStripe}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarInfoStripe"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarInfoStripe}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarWarningStripe"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarWarningStripe}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarDangerStripe"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarDangerStripe}" Value="40"></ProgressBar>
    </StackPanel>
    <StackPanel Margin="20">
        <TextBlock Text="ProgressBarFlat"></TextBlock>
        <ProgressBar Style="{DynamicResource ProgressBarFlat}" Value="40"></ProgressBar>
    </StackPanel>
```

effect:

![ProgressBar.Styles](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/native_controls/ProgressBar.Styles.png)

# Tips

For color, rounded corners or other custom requirements, please refer to [Progress Bar Style Source](https://github.com/HandyOrg/HandyControl/blob/master/src/Shared/HandyControl_Shared/Themes/Styles/ProgressBar.xaml)Define it yourself.