# 代码库收藏
> Bookmarks of some good repositories
>
> 记录我自己用过的, 或者是觉得还不错的库.
>
> Github自带的星标无法分组或管理, 索性就新挖了个库来做收藏

## Vue.js
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

#### [Akryum/vue-virtual-scroller](https://github.com/Akryum/vue-virtual-scroller)
> ⚡️ Blazing fast scrolling for any amount of data https://akryum.github.io/vue-virtual-…

#### [starkwang/vue-virtual-collection](https://github.com/starkwang/vue-virtual-collection)
>Vue component for efficiently rendering large collection data https://starkwang.github.io/vue-virtu…

#### [stackjie/vue-pull-to](https://github.com/stackjie/vue-pull-to)
>⚡️ A pull-down refresh and pull-up load more and infinite scroll component for Vue.js --Vue下拉刷新组件

下拉刷新组件, 能够控制下拉动作打开或关闭, 比mint-ui的loadmore要好用些. 

## Deep Learning 深度学习
#### [aidentify/lecture](https://github.com/aidentify/lecture)[韩文]
> 실습 강의 자료

朋友推荐的讲义, 由韩国公司**Aidentify**撰写

#### [aifriends](https://aifriends.github.io/) [韩文]
韩国大田市举办的AI论坛的日程发表网站

#### [케라스 강좌 내용](https://tykimos.github.io/lecture/) [韩文]
Keras韩国官网的管理人(?)所著写的书, 的Blog版本. 趣味生动的讲解了DeepLearning的基础, 以及Keras的使用.
适合新手入门.
