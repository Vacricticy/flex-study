# flex 弹性布局

## 一. 容器的六大属性

### 1. flex-direction 项目排列方向

- row（默认值） 主轴为水平方向
- column 主轴为垂直方向
- row-reverse
- column-reverse

### 2. flex-wrap 换行方式

- nowrap（默认） 不换行
- wrap 换行
- wrap-reverse

### 3. flex-flow

- flex-direction 与 flex-wrap 的结合

### 4. justify-content 主轴对齐方式

- flex-start（默认值）
- flex-end 右对齐
- center
- space-between 两侧对齐
- space-around 每个项目的间隔相等

### 5. align-items 交叉轴对齐方式

- flex-start 交叉轴的起点对齐
- flex-end 交叉轴的终点对齐
- center 交叉轴的中点对齐
- baseline 项目的第一行文字的基线 baseline 对齐
- stretch（默认值） 如果子项目未设置高度或设为 auto，将占满整个容器的高度。

### 6. align-content 多根轴线的对齐方式

- flex-start '整个内容'与交叉轴的起点对齐,与 align-items 不同的点就在于后者是将每一个子元素与交叉轴的起点对齐。
- flex-end 与交叉轴的终点对齐。
- center 与交叉轴的中点对齐。
- space-between 与交叉轴两端对齐，轴线之间的间隔平均分布。
- space-around 每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。
- stretch（默认值） 轴线占满整个交叉轴。

## 二. 单个项目的属性

### 1. order

- 默认值为 0，值越小，排列显示的顺序越靠前，可以取负值

### 2. flex-grow 空间有剩余时，怎样撑满

- 默认值为 0，即不撑满剩余的空间
- 若只有一个元素的 flex-grow 值为 1，则该元素撑满该行剩余的空间
- 若有多个元素设置了 flex-grow 值，则这些元素按比例来分割剩下的空间
- 若每个元素都设置了 flex-grow 值，则所有元素均按比例来分割剩下的空间

### 3. flex-shrink 空间爆炸时，怎么压缩

- 默认为 1，当元素在整行撑不下时，若没有设置 flex-wrap 为 wrap,则所有元素会等比例缩小来排下所有元素
- 若 flex-shrink 为 0，表示该元素不采用默认的缩小方式，会按原比例来显示
- 若大于 1，则按该值进行压缩

### 4. flex-basis

- 该元素先占据固有空间，剩余空间留给其他元素分割，默认值 auto 为原元素的大小，可设置值为 px 或%型

### 5. flex（一般采用这种形式）

- flex-grow flex-shrink flex-basis
- 默认值为 0 1 auto
- auto 表示 1 1 auto ; none 表示 0 0 auto

### 6. align-self

- 允许单个项目有与其他项目不一样的对齐方式，可覆盖 align-items 属性。

## 三. 应用

### 1. 骰子布局

### 2. 网格布局

- flex:0 0 10%

### 3. 圣杯布局

- 头部 header,尾部 footer,导航 nav，主栏 main,副栏 aside

### 4. 输入框的布局

### 5. 悬挂式布局

- 图片位置左（右）侧固定，剩余部分写内容

### 6. 固定的底栏

- 许可证

### 7 流式布局
