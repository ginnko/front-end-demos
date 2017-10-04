### Animation练习
计算随机生成的加减法题，使用Bootstrap布局。预览点击[此处]()。  

主要功能由以下组件完成：
- App.vue: Answer和Question两个组件的父组件，由<component>动态选择加载哪个组件；
- Question.vue: 生成随机数据、加减法、随机答案，由$emit传回控制条件；
- Answer.vue: 显示结果并重新开始下一题，由$emit传回控制条件。

动画使用transform: rotateY 在0~90°之间调整实现flip效果，代码用vue.js动画的基础方法写成。
