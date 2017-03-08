#图片画廊

###在线演示: https://pinmingkenan.github.io/gallery-by-react/

##安装运行

* 安装node.js环境
* 安装ruby环境
* 使用yeoman、webpack
* 安装yeoman: npm install -g yo
* 安装yeoman模板: npm install -g generator-react-webpack
* 自动生成项目: yo react-webpack gallery-by-react 
* 安装项目所有的依赖类库: npm install 
* 编辑 Main.js 开始项目

##发布项目

* 启动本地项目: npm start 或者 npm run serve
* 启动本地dist目录项目: npm run serve:start
* 打包到dist目录: npm run copy
* 清除dist文件：npm run clean
* 生成dist目录: npm run dist

* 删除dist目录中index.html中app.js的src中第一个斜杠
* 删除cfg目录中defaut.js中publicPath中的第一个斜杠

* 将文件全部添加到git仓库: git add -A  (git add dist)
* 提交代码: git commit -m 提交文件
* 推送代码大github上: git push
* 推送dist目录文件到githubPages: git subtree push --prefix=dist origin gh-pages 
* 回滚: git --hard 版本号

##CSS3翻转属性

* transform-style: preserve-3d; //3D加速
* transform: rotateY(180deg) scale(.5) translate(100px,20px) translateX(20px) skewY(12deg); //变形：翻转角度 缩放scale(x,y)默认基点是中心位置 位移 扭转角度
* transform-origin: left, top; //基点：位移trnsform发生的参照点
* transition: transform .6s easy-in-out, left .6s easy-in-out, top .6s easy-in-out 1s; //发生动画的过度,以,隔开，1s表延迟。
* perspective：3D环境中的井深（Z轴方向的基点距离平面的长度），perspective-origin基点；写在transform的父元素
* perspective:1800px; 最佳3D效果的位置
* Icon Font:字体文件 取代图片文件展示图片（1体积小，2支持css3属性变形）需在头部进行字体声明：@font-face{font-family:"";src:url() format(兼容)}
* CSS3伪元素&::after插入元素，而伪类的方式只需使用&:hover一个冒号
* at-root: 将css选择器提到最外层 (css中表示dom节点嵌套关系的标识)
* react 重新渲染时，是比较之前的结构和现在的结构，用key 给数组对应的一个值更快速的配对，加快性能

##调试技巧

* debugger();

##浏览器兼容
* chrome效果最佳

###觉得我写的不错的小伙伴，记得给我点赞哦^_^
