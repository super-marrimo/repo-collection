# 代码库收藏
> Bookmarks of some good repositories
>
> 记录我自己用过的, 或者是觉得还不错的库.
>
> Github自带的星标无法分组或管理, 索性就新挖了个库来做收藏

## Vue.js
### Vuex
#### [championswimmer/vuex-persist](https://github.com/championswimmer/vuex-persist)
> A Vuex plugin to persist the store. (Fully Typescript enabled) http://championswimmer.in/vuex-persist

将内存中Vuex的数据保存在localStorage的插件, 据说refresh不会丢失数据. 还没用过/

### Vue.js DateTime Picker

#### [vue-datetime](https://github.com/mariomka/vue-datetime)
> Mobile friendly datetime picker for Vue. Supports date, datetime and time modes, i18n and disabling dates.

用过的Datetime Picker里比较中规中矩, 发挥稳定的一款.

#### [vue-bootstrap-datetimepicker](https://github.com/ankurk91/vue-bootstrap-datetimepicker)
> Vue.js component for eonasdan-bootstrap-datetimepicker

### Chart

#### [ecomfe/vue-echarts](https://github.com/ecomfe/vue-echarts)
> ECharts component for Vue.js.

百度 Echart的VueJS 打包.

### List

#### [hilongjw/vue-recyclerview](https://github.com/hilongjw/vue-recyclerview)
> Mastering Large Lists with the vue-recyclerview https://hilongjw.github.io/vue-recycl…

List Item 不能自己控制, 只能将 component和data交给插件, 让他自己渲染, 这样导致component内部读取不到 $root, $router, $store 等常用Scope, 
尝试过将$store,$root中必要的数据和方法map到各个data里转交到component, 但使用起来总是用这样那样的问题.

component的位置由于是`position: absolute`, 高度在渲染之后是固定的, 在需要list Item 能够改变高度的的需求上力不从心(例如, item里有折叠内容之类).
适合轻量级的列表使用.

#### [tangbc/vue-virtual-scroll-list](https://github.com/tangbc/vue-virtual-scroll-list)
> ⚡️ A vue component support big data list with high scroll performance.

由variableHeigt函数获取每个子项目的高度并进行虚拟列表计算, 但variableHeight的调用时机和子项目dom的渲染时机不准确, 获取不到真实高度, 
所以一开始放弃使用.

但后来发现虚拟列表的动态高度计算能力都很差, (比如楼下的vue-virtual-scroller), 研究一番又回来尝试了一下,
才发现这个组件自定义功能比较丰富, 是个很有扩展力的组件. 对作者不禁心生佩服.
虚拟高度的计算也利用子项目自身的mounted函数来返回自身dom高度并实时更新列表来解决,  虽然还不是很完美, 但值得细细推敲.(谁叫11c的画面需求比较复杂)

#### [Akryum/vue-virtual-scroller](https://github.com/Akryum/vue-virtual-scroller)
> ⚡️ Blazing fast scrolling for any amount of data https://akryum.github.io/vue-virtual-…

VueJS的组件使用教程里有推荐到这个组件, 可以说是官方虚拟列表也不为过, 但由于结构比较复杂, 而且我对slot的各种嵌套很不熟悉, 最后没有能完成需求, 中途放弃. 
动态计算列表高度还是不完美.

作者似乎也是个牛人, chrome 的 Vue debug Tool 好像就是他开发的.

#### [starkwang/vue-virtual-collection](https://github.com/starkwang/vue-virtual-collection)
>Vue component for efficiently rendering large collection data https://starkwang.github.io/vue-virtu…

#### [stackjie/vue-pull-to](https://github.com/stackjie/vue-pull-to)
>⚡️ A pull-down refresh and pull-up load more and infinite scroll component for Vue.js --Vue下拉刷新组件

下拉刷新组件, 能够控制下拉动作打开或关闭, 比mint-ui的loadmore要好用些. 
更新: 发现被包含的组件里横向滚动似乎被禁止(或者是有影响), [11C]项目里列表中有横向滚动的相册组件, 所以放弃.

## Python
### 爬虫
#### [CriseLYJ/awesome-python-login-model](https://github.com/CriseLYJ/awesome-python-login-model)
😮python模拟登陆一些大型网站，还有一些简单的爬虫，希望对你们有所帮助❤️，如果喜欢记得给个star哦🌟

## Deep Learning 深度学习
#### [aidentify/lecture](https://github.com/aidentify/lecture)[韩文]
> 실습 강의 자료

朋友推荐的讲义, 由韩国公司**Aidentify**撰写

#### [aifriends](https://aifriends.github.io/) [韩文]
韩国大田市举办的AI论坛的日程发表网站

#### [케라스 강좌 내용](https://tykimos.github.io/lecture/) [韩文]
Keras韩国官网的管理人(?)所著写的书, 的Blog版本. 趣味生动的讲解了DeepLearning的基础, 以及Keras的使用.
适合新手入门.

#### [clone95/Machine-Learning-Study-Path-March-2019](https://github.com/clone95/Machine-Learning-Study-Path-March-2019)
Machine Learning 路线图.
