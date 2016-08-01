http://nate-river.github.io/blog/2016/05/08/Lear-Sass.html

10000小时定律
有效练习 ==  不舒服的练习


javascript
ruby python
node.js

pigments
color-picker

.darken   明度变的更暗
&:hover   引用上层的定义


&::after{
	content:"";
	clear:both;
}



@extned .btn
@extent %naem;
@mixin name{
	
}
@include name


混合宏

105em  
用 / 加括号
还可以加颜色        是将俩个的数值加起来   #ffff+#abc454



/**/
变量  默认值   局部变量
嵌套     &
继承/扩展    @extend
占位符       %
混合宏       @mixin name()    @include
插值        #{}
运算
注释


unquote
percentage   百分比
unquote   取空格
quote     加引号

round     
ceil    向上
floor
abs
min
max
random



length 取列表数据的长度
map 是重点、

clear:both    清除浮动的效果
content:
::after 让文档回到原来的效果




5.11 列表函数用法
length :($list)
nth:($list,3)
index: index($list,'seletor')


cursor:default;    鼠标光标的指针





@for 的循环方法

/*$lists: seletor,css,manipulation, traversing, events;
$color:red,blue,green,#acb456,#aca123;

  @for $i from 1 through length($lists){
    li.#{ nth($lists,$i) } {
        $tem:nth($color,$i);
        background: $tem;
        li:hover{
        background: black;
        color:$tem;
        }

    }
  }*/