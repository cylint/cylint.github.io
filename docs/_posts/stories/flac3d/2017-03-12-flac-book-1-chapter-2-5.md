---
layout: post
title:  "flac book 1 chapter 2.5"
tags: flac3d
categories: flac3d
---

* TOC
{:toc}


------

flac book 1 chapter 2.5

### fish 预定义变量

```
Igp
Jgp
Izones
Jzones
Clock   ;1/100s 计时
Unbal   ;最大不平衡力
Pi
Step
Urand   ;0-1随机均匀分布数据
```


### flac 内置函数

```
abs(a)
cos(a)
log(a)
max(a,b)
sqrt(a)

```

### 循环控制

设置弹性模量的非线性初始分布

E=E0+c*sqrt(z)


```
new
gen zone brick p0 (0,0,0) p1 (-10,0,0) p2 (0,10,0) p3 (0,0,-10)
model elas
plot set rotation 0 0 45
plot block group
def install
pnt = zone_head
  loop  while  pnt  #null
    z_depth = -z_zcen(pnt)
    y_mod = y_zero + cc * sqrt(z_depth)  
    z_prop(pnt, ’shear’) = y_mod / (2.0*(1.0+p_ratio))  
    z_prop(pnt, ’bulk’) = y_mod / (3.0*(1.0-2.0*p_ratio))  
    pnt = zone_next(pnt)  
  end_loop
end
set  p_ratio=0.25  y_zero=1e7  cc=1e8  
install
```

error

*** Property '0' not found in zone 1


