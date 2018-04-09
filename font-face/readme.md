# 关于字体的一些新认识

`font-weight`: 用来设置字体的粗细
`font-stretch`: 用来设置文字横向的紧窄程度(视觉上更瘦高或是扁平 condensed/expanded)

> 这两个属性并不会去改变字体本身的几何外形,而是在该字体家族中寻找合适的字体

比如 macOS 字体`pingfang sc`共有六种字重,分别是级细体,纤细体,细体,常规体,中黑体,中粗体.
设置不同的 `font-weight`会在该6种字重中根据某种算法来自动匹配具体的字重.
也就是说,**不同的`font-weight`值在视觉上不总是会有差异的**

```
/* Keyword values */
font-weight: normal;
font-weight: bold;

/* Keyword values relative to the parent */
font-weight: lighter;
font-weight: bolder;

/* Numeric keyword values */
font-weight: 100;
font-weight: 200;
font-weight: 300;
font-weight: 400;
font-weight: 500;
font-weight: 600;
font-weight: 700;
font-weight: 800;
font-weight: 900;
```
The font weights available to you will depend on the font-family you are using. Some fonts are only available in normal and bold.

```
/* Keyword values */
font-stretch: ultra-condensed;
font-stretch: extra-condensed;
font-stretch: condensed;
font-stretch: semi-condensed;
font-stretch: normal;
font-stretch: semi-expanded;
font-stretch: expanded;
font-stretch: extra-expanded;
font-stretch: ultra-expanded;

/* Global values */
font-stretch: inherit;
font-stretch: initial;
font-stretch: unset;
```

> 实测在 safari 上`font-stretch`可以使用百分比作为 value

`font-feature-settings`
对 otf 格式字体的高级印刷功能控制,更精细(可能更适合专门的字体设计师)
该属性是一个比较偏底层的功能接口，用于解决由于没有其他方法去访问和设置OpenType字体某些特性而无法解决一些特殊功能需求.
The `font-feature-settings` CSS property gives you control over advanced typographic features in OpenType fonts.

`font-variant`
一些高级控制,更精细(可能更适合专门的字体设计师)
The font-variant CSS property is a shorthand for the longhand properties font-variant-caps, font-variant-numeric, font-variant-alternates, font-variant-ligatures, and font-variant-east-asian