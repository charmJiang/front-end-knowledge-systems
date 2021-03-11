### 前端存在的历史问题

![x8CxMk](https://gitee.com/vr2/images/raw/master/uPic/x8CxMk.png)

1. 1v1页面taro跟单独方案（taro/plans）页面，是2个工程，有新相同的需求需要维护2套工程
2. （c端）技术栈不统一，新来人员无法快速融入业务开发，增加成本





### 需求开发存在的问题：

#### **转介绍活动**

**1.存在的问题**：

- 如果在原有的1v1页面上开发，代码过于臃肿；
- 如果增加单独的活动，每个活动上线，都得重新部署
- 在原有的1v1上修改，后续项目改造，得重新写代码，无法共用。

**2.解决的方案**：

- 转介绍活动过，通过新加工程开发

**3.成本：**

- 容器成本
- 项目前期需要花费时间，搭建项目
- 测试需要全部走流程

**4.好处**

- 所有的活动项目可以在同一的工程上开发
- 支持单独部署，影响用户体验较少
- 代码不会混在一起，代码优雅
- 业务统一



#### 问卷优化	

**1.存在的问题：**

- 问卷页面需要修改
- 单独方案页需要修改
- 1v1方案页需要修改

**2.解决方案**

- 新增工程

- 将单独方案页， 1v1和问卷优化工程融合到一起

**3.好处**

- 维护成功提高
- 改善用户体验





### 总体方案

方案1:

![EnFB0g](https://gitee.com/vr2/images/raw/master/uPic/EnFB0g.png)



- 将1v1，问卷，单独方案页融合在一个工程，独立维护，作为一个主应用
- 转介绍（其他）活动做为一个1应用，单独维护，部署。

**方案2:**

![2GJ8SI](https://gitee.com/vr2/images/raw/master/uPic/2GJ8SI.png)



- 将1v1作为一个主应用，问卷和转介绍活动，拆分成不用子应用，支持主，子应用相互跳转

  










