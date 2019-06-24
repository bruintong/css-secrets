# CSS 揭秘

## 背景和边框
- [透明边框](./background-border/translucent-borders.html)：默认情况下，背景会延伸到边框所在的区域下面，可以通过 **background-clip** 属性来调整默认行为。
- [多重边框](./background-border/multiple-borders.html)：使用 **box-shadow** 来模拟外框，模拟的边框出现在在外圈，并不会响应鼠标事件，可以给 **box-shadow** 属性加上 **inset** 关键字，来使投影绘制在元素的内圈。
- [灵活的背景定位](./background-border/extended-bg-position.html)：**background-position** 允许指定背景图片距离任意角的偏移量，只要在偏移量前面指定关键词。
- [灵活的背景定位](./background-border/background-origin.html)：默认情况下，**background-position** 是以 **padding-box** 为准的，可以使用 **background-origin** 来改变该基准。
- [灵活的背景定位](./background-border/background-position-calc.html)：使用calc()函数计算偏移值进行背景定位。
- [边框内圆角](./background-border/inner-rounding.html)：利用描边 **outline**不跟着圆角走的事实，配合 **box-shadow** 实现边框内圆角。
- [条纹背景-水平条纹](./background-border/horizontal-stripes.html)：使用线性渐变 **linear-gradient** 将两个色标重合可以创建实色条纹。如果某个色标的位置值比整个列表中在它之前的色标值都要小，则该色标的位置值会被设置成它前面所有色标位置的最大值。这意味着，如果把第二个色标的位置设置为0，那它的位置就总是被浏览器调整为前一个色标的位置值。
- [条纹背景-垂直条纹](./background-border/vertical-stripes.html)：垂直条纹的代码跟水平条纹几乎是一样的，差别主要在于:我们需要在 开头加上一个额外的参数来指定渐变的方向。
- [条纹背景-斜向条纹](./background-border/diagonal-stripes.html)：斜向条纹不但能简单通过改变渐变方向得到，原因在于只是把每个“贴片”内部渐变旋转了45度，而不是把整个重复的背景都旋转了。单个贴片包 含了四条条纹，而不是两条，只有这样才有可能做到无缝拼接。
- [条纹背景-更好的斜向条纹](./background-border/diagonal-stripes-60deg.html)：利用 **repeating-linear-gradient** 可以轻易实现任意角度的斜向条纹。
- [条纹背景-更好的斜向条纹](./background-border/test-color-stop-2positions.html)：利用 **repeating-linear-gradient** 可以在同一个色标上指定两个位置值相当于两个连续的色标具有相同的颜色和不同的位置，这个特性在创建渐变图案时是十分有用的。
- [灵活的同色系条纹](./background-border/subtle-stripes.html)：最深的颜色指定为背景色，同时把半透明白色的条纹叠加在背景色之上来 得到浅色条纹。
- [复杂的背景图案](./background-border/blueprint.html)：水平渐变图案跟垂直渐变图案配合实现简单的蓝图网格图案。
- [波点](./background-border/polka.html)：径向渐变创建最简单的圆点的阵列。
- [棋盘](./background-border/checkerboard.html)：用两个直角三角形来拼合出方块。
- [棋盘](./background-border/checkerboard-svg.html)：用SVG来实现棋盘效果。
- [伪随机背景](./background-border/cicada-stripes.html)：通过质数来增加随机真实性。
- [连续的图像边框](./background-border/border-image.html)：**border-image** 基本原理就是九宫格伸缩法：把图片切割成九块，然后把它们应用到元素边框相应的边和角。
- [连续的图像边框](./background-border/continuous-image-borders.html)：**border-image** 基本原理就是九宫格伸缩法：把图片切割成九块，然后把它们应用到元素边框相应的边和角。
- [老式信封样式边框](./background-border/vintage-envelope.html)：利用渐变实现老式信封样式边框。
- [蚂蚁行军边框](./background-border/marching-ants.html)：虚线边框动画。
- [脚注](./background-border/footnote.html)：脚注。

## 形状
- [自适应的椭圆](./shape/ellipse.html)：**border-radius** 可以单独指定水平和垂直半径，只要用一个斜杠（/）分隔这两个值即可。这个特性允许在拐角处创建椭圆圆角。
- [半椭圆](./shape/half-ellipse.html)
- [四分之一椭圆](./shape/quarter-ellipse.html)
- [平行四边形](./shape/parallelograms.html)：通过skew的变形属性对矩形进行拉伸。
- [平行四边形](./shape/parallelograms-pseudo.html)：利用伪元素以及定位属性产生一个方块，然后对伪元素设置样式，并将其放置在其宿主元素对下层。当想变形一个元素而不想变形它对内容时非常有用。
- [菱形图片](./shape/diamond-images.html)：通过rotate变形 + scale变形实现菱形图片，旋转后图片的宽度应与容器对角线相等。
- [菱形图片-裁剪路径](./shape/diamond-clip.html)：**clip-path** 属性可以把元素裁剪成任何形状。
- [切角效果](./shape/bevel-corners-gradients.html)：利用线性渐变实现切角效果。
- [切角效果](./shape/bevel-corners.html)：利用SVG实现切角效果。
- [切角效果](./shape/bevel-corners-clipped.html)：利用 **clip-path** 实现切角效果。
- [弧形切角](./shape/scoop-corners.html)：利用径向渐变实现弧形切角。
- [梯形标签页](./shape/trapezoid-tabs.html)：3D旋转模拟梯形标签页。
- [简单饼图-基于transform的解决方案](./shape/pie-animated.html)：进度指示器
- [静态饼图](./shape/pie-static.html)：用负的动画延时来直接跳至动画中的任意时间点，并且定格在那里。
- [静态饼图-SVG](./shape/pie-svg.html)

## 视觉效果
- [单侧投影](./visual-design/shadow-one-side.html)：利用 **box-shadow** 的第四个长度参数，扩张半径，这个参数会根据你指定的值去扩大或（当指定负值时）缩小投影的尺寸。
- [邻边投影](./visual-design/shadow-2-sides.html)
- [双侧投影](./visual-design/shadow-opposite-sides.html)：用两块投影（每边各一块）来实现双侧投影的目的。
- [不规则投影](./visual-design/shadow-opposite-sides.html)：使用 **drop-shadow** 滤镜实现投影，任何非透明的部分都会被一视同仁地打上投影，包括文本，并且无法通过 **text-shadow:none;** 来取消掉文本上的投影。
- [染色效果](./visual-design/color-tint-filter.html)：叠加滤镜效果的方式实现染色效果。
- [染色效果-基于混合模式](./visual-design/color-tint.html)：当两个元素叠加时，混合模式控制了上层元素的颜色与下层颜色进行混合的方式。
- [毛玻璃效果](./visual-design/frosted-glass.html)：把文本层所覆盖的那层图片区域作模糊处理。
- [折角效果](./visual-design/folded-corner.html)：叠加线性渐变实现折角效果。
- [折角效果-伪元素](./visual-design/folded-corner-realistic.html)：更加真实的折角效果。

## 字体排版
- [连字符断行](./font-type/hyphenation.html)：hyphens:auto; 无效果。
- [插入换行](./font-type/line-breaks.html)：通过伪元素插入。
- [文本行斑马条纹](./font-type/zebra-lines.html)：直接通过渐变生成背景图像。
- [调整tab的宽度](./font-type/tab-size.html)：CSS属性tab-size控制。
- [连字](./font-type/ligatures.html)：CSS属性font-variant-ligatures控制连字效果。
- [华丽的&符号](./font-type/ligatures.html)：通过指定特定字符的@font-face实现。
- [自定义下划线](./font-type/underlines.html)：使用渐变来实现下划线。
- [波浪型下划线](./font-type/wavy-underlines.html)：使用渐变来实现波浪型下划线。
- [现实中的文字效果](./font-type/letterpress.html)：对深色底浅色字使用凸版效果。
- [空心字效果](./font-type/stroked-text.html)：使用SVG实现空心字效果。
- [文字外发光效果](./font-type/glow.html)：使用text-shadow或滤镜blur实现模糊效果。
- [文字凸起效果](./font-type/extruded.html)：使用一长串累加的投影，不设模糊并以1px的跨度逐渐错开，使颜色逐渐变暗，然后在底部加一层强烈模糊的暗投影。
- [环形文字](./font-type/circular-text.html)：SVG实现环形文字。

## 用户体验
- [选用合适的鼠标光标](./user-experience/disabled.html)：不可用状态、隐藏鼠标。
- [扩大可点击区域](./user-experience/hit-area-border.html)：Fitts法则认为，人类移动到某个目标区域所需的最短时间是由目标距离与目标宽度之比所构成的对数函数。透明边框扩大热区，**background-clip：padding-box** 将背景限制在原本的区域之内。按钮需要真正的边框效果时，使用内嵌投影来模拟边框。
- [扩大可点击区域-伪元素](./user-experience/hit-area.html)：伪元素同样可以代表其宿主元素来响应鼠标交互。
- [自定义复选框](./user-experience/checkboxes.html)：<label>元素与复选框关联，借助 **:checked** 选择符来给元素设置样式。
- [开关式按钮](./user-experience/toggle-buttons.html)：复选框模拟按钮。
- [通过阴影来弱化背景](./user-experience/dimming-box-shadow.html)：**box-shadow**只能在视觉上起到引导注意力的作用，无法阻止鼠标交互。
- [backdrop方案](./user-experience/native-modal.html)：使用<dialog>元素，浏览器对它支持很有限。
- [通过模糊来弱化背景](./user-experience/deemphasizing-blur.html)：使用滤镜产生景深效果。
- [滚动提示](./user-experience/scrolling-hints.html)：使用渐变实现阴影和配套的遮罩。
- [交互式的图片对比控件](./user-experience/image-slider.html)：**resize**可以限制元素调整大小的方向。

## 结构与布局
- [自适应内部元素](./structure-layout/intrinsic-sizing.html)：**min-content** 关键字解析为这个容器内部最大的不可断行元素的宽度。
- [精确控制表格列宽](./structure-layout/table-column-widths.html)：**table-layout: fixed** 固定表格布局算法让表格布局更加可控。
- [根据兄弟元素的数量来设置样式](./structure-layout/styling-sibling-count.html)
- [满幅的背景，定宽的内容](./structure-layout/fluid-fixed.html)：使用内边距实现水平居中布局
- [垂直居中](./structure-layout/vertical-centering-abs.html)：绝对定位 + 变形属性来实现。translate变形函数中使用百分比值时，是以这个元素自身的宽度和高度为基准进行换算和移动的。
- [垂直居中](./structure-layout/vertical-centering-vh.html)：基于视口单位的解决方案，margin的百分比值是以父元素的宽度作为解析基准的。
- [垂直居中](./structure-layout/vertical-centering.html)：基于Flexbox的解决方案。当我们使用Flexbox时，margin：auto不仅在水平方向上将元素居中，垂直方向上也是如此。
- [紧贴底部的页脚](./structure-layout/sticky-footer-fixed.html)：页脚高度固定
- [紧贴底部的页脚](./structure-layout/sticky-footer.html)：基于Flexbox的解决方案，让内容区块的高度可以自动伸缩并占满所有的可用空间。

## 过渡与动画
- [小球回弹动画](./transition-animation/bounce.html)：通过三次贝塞尔曲线来指定动画曲线。
- [弹性过渡](./transition-animation/elastic.html)：提示框动画。
- [逐帧动画](./transition-animation/frame-by-frame.html)：step调速函数，step会根据指定的步进数量，把整个动画切分为多帧，而且整个动画会在帧与帧之间硬切，不会做任何插值处理。
- [闪烁效果](./transition-animation/blink.html)：平滑的闪烁动画。
- [打字动画](./transition-animation/typing.html)：在等宽字体中，“0”字形的宽度和其他所有字形的宽度是一样的，可以使用ch单位表示。
- [状态平滑的动画](./transition-animation/state-animations.html)：暂停和继续一个一直存在的动画。
- [沿环形路径平移的动画](./transition-animation/circular-2elements.html)：2个元素实现环形路径平移的动画
- [沿环形路径平移的动画](./transition-animation/circular.html)：**transform-origin** 只是一个语法糖而已。实际上你总是可以用 **translate()** 来代替它。

## 参考手册
- [CSS3 简介](./reference/intro.html)
- [关键字](./keyword.html)