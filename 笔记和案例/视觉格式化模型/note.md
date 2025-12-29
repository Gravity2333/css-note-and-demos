视觉格式化模型是视觉媒体上展示文档的计算规则
也就是 把 元素 转换为页面上具体位置盒子的一套规则
Css盒模型计算盒子的尺寸
视觉格式化模型计算页面如何布局这些盒子


BFC
1. 块盒之间垂直排布
2. 块盒之间的距离通过margin设定，父子元素 相邻块元素垂直方向 空块元素上下margin会合并
3. 子元素沿着BFC左侧边排布
4. BFC和float不重叠
5. BFC计算高度的时候 浮动被计算在内 定位排除 所以无法解决定位塌陷 可以解决浮动塌陷
6. 内部对外部没有任何影响

如何产生
inline-block
float
绝对定位 absolute fixed
flow-root
grid
flex
overflow 非 visivle


IFC 
1. 行内盒子水平排布
2. margin padding 水平方向影响其他行内盒子，垂直方向只渲染 不改变布局
3. 在换行位置会阶段 margin padding
4. 行盒 剩余空间用 text-align 分配
5. 行盒 高度通过line-height & vertical-align 共同决定
6. 浮动盒子优先排布，排布后再排布行盒

IFC通过容器盒子生成

