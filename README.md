# svg
some demo

**SVG 文件必须使用 .svg 后缀来保存**

***
* `<?xml version="1.0" standalone="no"?>`
包含了 XML 声明。请注意 standalone 属性！该属性规定此 SVG 文件是否是“独立的”，或含有对外部文件的引用。
standalone="no" 意味着 SVG 文档会引用一个外部文件 - 在这里，是 DTD 文件。 

***
* `<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" 
"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<svg width="100%" height="100%" version="1.1"
xmlns="http://www.w3.org/2000/svg">`
引用了这个外部的 SVG DTD。该 DTD 位于 “http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd”。该 DTD 位于 W3C，含有所有允许的 SVG 元素。
1. SVG 代码以 <svg> 元素开始，包括开启标签 <svg> 和关闭标签 </svg> 。这是根元素。
2. width 和 height 属性可设置此 SVG 文档的宽度和高度。
3. version 属性可定义所使用的 SVG 版本，
4. xmlns 属性可定义 SVG 命名空间。

***
**`<circle>` 标签 圆形**
* `<circle cx="100" cy="50" r="40" stroke="black"
stroke-width="2" fill="red"/>`
SVG 的 <circle> 用来创建一个圆。
1. cx 和 cy 属性定义圆中心的 x 和 y 坐标。如果忽略这两个属性，那么圆点会被设置为 (0, 0)。
2. r 属性定义圆的半径。
3. stroke 和 stroke-width 属性控制如何显示形状的轮廓。我们把圆的轮廓设置为 2px 宽，黑边框。
4. fill 属性设置形状内的颜色。我们把填充颜色设置为红色。
***
**`<rect>` 标签 矩形**
<rect> 标签可用来创建矩形，以及矩形的变种。
1. rect 元素的 width 和 height 属性可定义矩形的高度和宽度
2. style 属性用来定义 CSS 属性
3. CSS 的 fill 属性定义矩形的填充颜色（rgb 值、颜色名或者十六进制值）
4. CSS 的 stroke-width 属性定义矩形边框的宽度
5. CSS 的 stroke 属性定义矩形边框的颜色
6. x 属性定义矩形的左侧位置（例如，x="0" 定义矩形到浏览器窗口左侧的距离是 0px）
7. y 属性定义矩形的顶端位置（例如，y="0" 定义矩形到浏览器窗口顶端的距离是 0px）
8. CSS 的 fill-opacity 属性定义填充颜色透明度（合法的范围是：0 - 1）
9. CSS 的 stroke-opacity 属性定义笔触颜色的透明度（合法的范围是：0 - 1）
10. rx 和 ry 属性可使矩形产生圆角。
***
**`<ellipse>` 标签 椭圆**
1. cx 属性定义圆点的 x 坐标
2. cy 属性定义圆点的 y 坐标
3. rx 属性定义水平半径
4. ry 属性定义垂直半径
***
**`<line>` 标签 线条**
1. x1 属性在 x 轴定义线条的开始
2. y1 属性在 y 轴定义线条的开始
3. x2 属性在 x 轴定义线条的结束
4. y2 属性在 y 轴定义线条的结束
***
**`<polygon>` 标签 多边形**
1. points 属性定义多边形每个角的 x 和 y 坐标
***
**`<polyline>` 标签 折线**
***
**`<path>` 标签 路径**
* 下面的命令可用于路径数据：
1. M = moveto
2. L = lineto
3. H = horizontal lineto
4. V = vertical lineto
5. C = curveto
6. S = smooth curveto
7. Q = quadratic Belzier curve
8. T = smooth quadratic Belzier curveto
9. A = elliptical Arc
10. Z = closepath
######注释：以上所有命令均允许小写字母。大写表示绝对定位，小写表示相对定位。
