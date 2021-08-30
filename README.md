# el-virtual-tree
el-tree 支持虚拟滚动

### Attributes、props、方法、Events
与 [el-tree](https://element.eleme.cn/#/zh-CN/component/tree) 一致

### 依赖插件
``vue-virtual-scroll-list``

### 使用方法（使用前请确认已引入 [element-ui](https://element.eleme.cn/#/zh-CN/component/tree) ）
#### 第一步 安装依赖
``npm i vue-virtual-scroll-list``

#### 第二步 导入组件
在你的项目组件目录中（一般为``src/components``）新建文件夹``el-virtual-tree``，
将本项目所有文件粘贴至该文件夹

按需引入

``import ElVirtualTree from '@/src/components/el-virtual-tree'``

vue components引入组件``components: { ElVirtualTree }``

或者全局引入
````
import Vue from 'vue';
import ElVirtualTree from '@/src/components/el-virtual-tree;

Vue.use(ElVirtualTree)
````

### 使用说明
设置组件高度``height``属性开启虚拟滚动，否则不开启。

``height``属性为字符类型，需自带单位，例：``height="300px"`` ``height="calc(100vh - 200px)"``

### 完整例子
````
<el-virtual-tree
:data="treeData"
node-key="id"
height="calc(100vh - 210px)" // 设置该属性则开启虚拟滚动
>
...
</el-virtual-tree>
```
