1.引入所需的文件
  css & js
2. 根据插件的规定 写好基本的dom结构
3. 开始制作页面
   要制作的页面又各种各样的需求
   所以需要给插件添加一些配置项
  ````````javascript```````````
  $(function(){
      $('#main').fullpage({
          scrollingSpeed:400,     //滚动一屏的时间
          anchors:['youxing','shiping'],   //index.html#jiewei(分享给别人)
          fixedElements:'#fix,.header nav',
          paddingTop:20,
          paddingBottom:30,
          //当滚动到底部之后或顶部之后能不能继续滚动
          continuousVertical:true,
          //是否出现导航小店
          navigation:true,
          //每一个小点的提示文字
          navigationTooltips:['a','b','c','d'],
          // 到一屏的时候是否出现提示文字
          showActiveTooltip:true,
          // 进入一屏的时候 会调用afterLoad
          afterLoad:function(name,index)
          //// name是当前的名字 index是第几张
          onLeave:function(index,next,dir)
           //index 从那张离开
           // naxt 取到了那张
           // dir  方向  up  down 
           eg：
              onLeave:function(index,next,dir){
               if( index ===5 ){
                   $(;#section h1).addClass('animate-fei')

           }
           if(index === 1){
           	  // 离开失效 
           	  return false;
           }
          }
            
      })
  })

  ##4.使用css结合js起制作页面中的动画
     一、 使用transtion结合fullpage 去制作动画
      ```````transition:transform .5s ease 1s ,opacity .6s ease-in-out .5s
              transform:  rotateX()
              transform:  rotateY()
              transform:  rotateZ()
              || transform:retoteX() scale(0.3,0.3);
              transform: translate3d(30px,20px,0)  retateZ(34deg)
     1. 要动的元素写到每一个section中
     2. 正常状态下的一中样子
     3. 当section 有了action  fp-complately类之后的另一个样子
     4. 给要动的元素加上那个 transition 检测
     二、
     ······使用animation j结合fullpage取制作动画
     animated 简写的主义事项
      ···
      name:fei
      duration:3s
      timing-function:ease
      delay:5s
      fill-mode:both
      direction：alternate   //运动方向   来回
      iteration-count:infinite
      play-state:running || paused
      `````
      $('#ani').get(0).style.animated
     1. 要动的元素写到每一个section中
     2.正常状态下的采用的一种动画
     3.在section 拥有active 类情况下采用另一种动画
     4.一些更复杂的情况 把动画预先写好 
