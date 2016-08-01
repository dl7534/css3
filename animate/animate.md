transition-property: all;

永远不要写all 会增加工作量  写那些真正需要的变量


transition:
ease
ease-in
ease-in-out
ease-out
liner
step-end
step-start
steps(10,start)
cubic-bezier()   贝塞尔曲线
1001

 #transition .delay-list{
	li{
	  width:100px;
	  height:50px;
	  border:1px solid #000;
	  margin-bottom:3px;
	  width:300px;
	  position: relative;
	  left:-100px;
	  transition-property:left,background;
	  transition-duration:0.3s;
	  transition-timing-function: ease-in;
	  }
}
	#da:checked + .delay-list li{	
		  	left:50%;
		  	background: red;
	}
	@for $i from 1 through 4 {
          	 li:nth-child(#{$i}){
          	 transition-delay: $i*0.3s;
          }
}




https://github.com/getlantern/lantern   蓝灯下载地址


<!--  -->
node-sass 安装教程(破解版)
npm install -g yo
npm install -g generator-webapp
npm install -g node-sass
npm install -g bower
nom install -g grunt-cli
nom install -g gulp-cli
yo webapp



在apple中的文字设为 width：1 height：1 overflow:hidden;  不是设为display:none    是为了tab键可以切换 处理





https://github.com/alvarotrigo/fullPage.js  老师讲作品   重要