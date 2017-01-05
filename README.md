安装运行

使用yoman、webpack

npm install yo -g
npm install generator-react-webpack -g
yo react-webpack gallery-by-react 自动生成项目
运行 node server.js
npm install autoprefixer-loader --save-dev
编辑 Main.js 开始项目
发布项目
打包到dist目录npm run copy & webpack --env=dist
git add \git commit
git subtree push --prefix=dist origin gh-pages 推送到Github提供的静态文件访问上
访问http://xiaoqiany.club/gallery-by-react/
知识点

CSS3翻转属性

transform-style:preserve-3d; //3D加速
transform:rotateY(180deg) scale(.5) translate(100px,20px)\translateX(20px) skewY(12deg); //变形：翻转角度 缩放scale(x,y)默认基点是中心位置 位移 扭转角度
transform-origin:left,top; //基点：位移trnsform发生的参照点
transition:transition .6s easy-in-out, left .6s easy-in-out,top .6s easy-in-out 1s; //发生动画的过度,以,隔开，1s表延迟。
perspective：3D环境中的井深（Z轴方向的基点距离平面的长度），perspective-origin基点；写在transform的父元素上。
perspective:1800px;
Icon Font:字体文件 取代图片文件展示图片（1体积小，2支持css3属性变形）需在头部进行字体声明：@font-face{font-family:"";src:url() format(兼容)}
CSS3伪元素&::after插入元素，而伪类的方式只需使用&:hover一个冒号。
react 重新渲染时，是比较之前的结构和现在的结构，用key 给数组对应的一个值更快速的配对，加快性能。
调试技巧

debugger();
