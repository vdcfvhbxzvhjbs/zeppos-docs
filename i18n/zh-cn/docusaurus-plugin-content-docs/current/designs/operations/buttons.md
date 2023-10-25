---
sidebar_label: 按钮
--- 

# 按钮  

按钮是一个具有明确指示动作的交互元件 。它可以触发功能、引导用户操作并有助于形成用户心智。

## 设计原则  

- 按钮表意需要清晰易懂，帮助用户快速了解它的意图。
- 为按钮交互提供反馈，减少用户不必要的操作，提高使用效率。
- 保证按钮的可点击区域，由于可穿戴设备屏幕大小限制，对于较小的按钮，请扩大按钮的可点击区域，保证用户操作的准确率。
- 避免使用太多按钮，请务必控制页面中按钮数量，考虑最重要的操作，控制好优先级和复杂度。
- 注意按钮顺序，页面中按钮的顺序遵循方向性原则，符合用户对话习惯；保证按钮的顺序一致，不仅利于提升用户的操作效率，同时会减少用户的操作出错概率。

## 悬浮按钮  

固定悬浮在页面最上层显示，不支持跟随页面滑动，具有较强告知属性。

![Design](/img/design/f8b8a043408d2ee489d71795593c4ca2.png)

![Design](/img/design/9db22be976265dd72d7c6ff097f8b149.png)

## 胶囊按钮  

页面中常见的按钮样式，按钮会跟随界面滑动，按照使用场景分为➀默认按钮、②强调按钮和③警示按钮。  

![Design](/img/design/821e6b022c6c057855294a465fe88224.png)  

## 圆形按钮  

通过承载视觉图形来传达按钮意图，可以在较小的屏幕空间内展示更多内容。请控制不同尺寸的圆形按钮在页面上的数量。  

![Design](/img/design/88c02b58be7a502f9f6d0186f57f01b6.png)  

## 图标按钮  

相比圆形按钮，视觉层级更为轻量化的按钮形式；图标按钮可以节省界面空间，但需要注意尽量不要用图标按钮来做复杂表意。  

![Design](/img/design/8cb66d7c277e8bd138fef75a7ebbfc6f.png)  

## 文字按钮  

由于文字按钮没有容器，它们不会分散附近内容的注意力，视觉感受较弱。文字按钮通常用于不太明显的操作。  

![Design](/img/design/454dc39d-ddc0-466f-8f3b-ab5206865e0a.png)  

## 使用规则   

- 根据当前按钮交互行为的层级性，同时考虑屏幕空间大小和整体布局来选用恰当的按钮样式。
- 按钮文案应保持简练，胶囊按钮文案长度极限支持两行。  

![Design](/img/design/f0a1b035e4ab0e0c592731b0ad0cd22f.png)

- 按钮文案两行极限字数尽量控制在（“A”字符为例）为26个字符以内，文本超长两行显示不下，使用“...”结尾省略显示。  

![Design](/img/design/buttons-rules-for-use.png)  

>① 极限字符数示意
>
>② 超长显示样式


- 英文文案避免全部大写而降低识别速度  

![Design](/img/design/avoid-all-caps.png)  

-  按钮可通过添加关键色告知进度状态，例如：离线语音唤设定闹钟，建议使用悬浮按钮并明确告知倒计时进度。  

![Design](/img/design/4c7538d6c0dddb75dc43234b7c6b45b2.png)

## 视觉规范 

关于方屏与圆屏设备按钮的差异性：方屏与圆屏设备按钮规格各有不同，设计时请分别调用对应组件库按钮组件，规格区别详情见下方示例。  

- 方屏与圆屏设备对应悬浮按钮样式。  

![Design](/img/design/9168f0921543809043346ba7042e02ed.png)

- 方屏与圆屏设备胶囊按钮尺寸区别。  

![Design](/img/design/3d41fd78e3e8e24dc7420aa817cc5e58.png)  

>➀圆屏设备  
>
>②方屏设备  

- 圆形按钮分六种尺寸，同一个按钮在圆屏和方屏两种设备中时，其尺寸不变。绘制切图请遵循图标对应尺寸规范 （较小尺寸图标按钮建议扩大点击区域，尺寸不得小于64px规格）。  

![Design](/img/design/c5e786bdd6c3832b798ece0176b7f866.png)

- 按钮状态与色值定义按照规范设定。  

![Design](/img/design/15cf2e946c828842927ec9439f9c9a2b.png)

 >➀默认按钮底色：color_sys_button_bg   文字/图标：color_text_button
 >
 >②强调按钮底色：color_sys_key   文字/图标：color_text_button
 >
 >③带有特殊属性按钮颜色遵循色彩规范定义色值，例如：来电、删除按钮   

![Design](/img/design/7714d6ffd05a28508360a921b16f4a7b.png)

>④文本按钮色值：color_text_link  

- 在触发点按动作时，按钮整体颜色亮度降低 28.6%。  

![Design](/img/design/424672ce8de01374da6b5fb21374099c.png)

 >➀有色按钮默认与点击状态   ②无色按钮默认与点击状态。