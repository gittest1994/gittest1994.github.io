---
title: Globalization
---

# Way of use

The language package to be used can be specified by `ConfigHelper.Instance.SetLang(string lang)`, English (en) is used by default.

The language package that comes with the control library is generally used internally by the control library, but users can also use it in the following two ways:

- xaml
The first step is to introduce the namespace: `xmlns:hc="https://handyorg.github.io/handycontrol"`
The second step is to use the language pack: `<TextBlock Text="{x:Static hc:Lang.Cancel}"/>`

- C#
`HandyControl.Properties.Langs.Lang.Cancel`

{% note warning %}
The control library does not support dynamic language package switching, and there will be no support in the future.
{% endnote %}

# Language packs

The language packs included with the control library include:

* Simplified Chinese (zh-cn)
* English (en)
* Persian (fa)
* French (fr)
* Korean (ko-kr)

`The default is English (en).`

If you need to expand on your own, it is recommended to use the open source plugin: [ResXManager](https://marketplace.visualstudio.com/items?itemName=TomEnglert.ResXManager) to maintain all language packs.

After the control library is referenced, the language package folder is generated in the running directory, and its naming style is like zh-cn, en, and so on.