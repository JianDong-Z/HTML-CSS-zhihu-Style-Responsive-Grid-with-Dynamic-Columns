卡片式布局，模仿知乎的动态网格设计

问题：当Grid布局的列数超过容器宽度时，如何避免内容溢出？
回答：使用minimax(300px,1fr)约束最小列宽，配合auto-fit自动调整列数，同时设置overflow-x:auto允许横向滚动

使用 grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)) 实现 动态列数
图文混排时锁定图片比例（aspect-ratio属性），解决布局错位问题
通过 gap 替代 margin 提升代码可维护性