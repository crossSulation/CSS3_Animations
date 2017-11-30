# CSS3_Animations
Some demos and knowlage about CSS3 Animation
# Animation 参考https://www.w3schools.com/cssref/css3_pr_animation.asp
1)animation 语法
针对不同的内核的浏览器，需要加上相应的前缀
-webkit-animation,-ms-animation,-o-animation,-mz-animation,-or-

#综合使用
animation: name duration timing-function delay iteration-count direction fill-mode play-state;

name 是指通过 @-webkit-keyframes (@keyframes) 定义的帧动画
duration 动画持续时间以秒为单位的 number类型
timing-function 动画执行效果函数,常用的有 ease, linear,ease-in,ease-in-out.下面单独使用改属性时会详细解答
delay 动画停顿时间，默认值是 0，单位为秒(s)
iteration-count 动画循环执行次数，默认是1, 如果指定infinite,动画则无限循环
direction 动画运动方向 ，可以设置值，normal,reverse,alternate,alternate-reverse,initial,inherit
fill-mode 指定动画开始前或者动画结束后，或者动画开始前和结束后元素(element)的样式，因为单纯使用animation不能指定动画开始前或结束后的style,使用这个属性可以达到目的
play-state 指定动画的运行状态，值可以是paused,running,initial,inherit

#单独使用上面的属性

animation-name 使用 keyframe中指定的帧动画(keyframename)
#CSS synax
animation-name: keyframename|none|initial|inherit;

animation-duration 动画持续时间, time可以是妙(s)，毫米(ms)
#CSS synax
animation-duration: time|initial|inherit;

animation-timing-function 动画效果函数 
#CSS synax 
animation-timing-function: linear|ease|ease-in|ease-out|ease-in-out|step-start|step-end|steps(int,start|end)|cubic-bezier(n,n,n,n)|initial|inherit;

animation-delay 指定动画启动前停顿时间,time可以是(s),(ms)
#CSS synax
animation-delay: time|initial|inherit;

animation-iteration-count : 动画循环次数
#CSS synax
animation-iteration-count: number|infinite|initial|inherit;

animation-direction 动画运动方向
#CSS synax
animation-direction: normal|reverse|alternate|alternate-reverse|initial|inherit;

animation-fill-mode 指定动画开始前或动画结束后，元素的style
#CSS synax
animation-fill-mode: none|forwards|backwards|both|initial|inherit;

animation-play-state 动画运行状态, paused or running
#CSS synax
animation-play-state: paused|running|initial|inherit;











#@keyframes 参考https://www.w3schools.com/cssref/css3_pr_animation-keyframes.asp