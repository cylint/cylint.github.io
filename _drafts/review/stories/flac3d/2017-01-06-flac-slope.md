---
title: "Flac slope"
tags: flac3d
categories: flac3d
---



## 快速入门

print memory system

print mem sav mem sys

模型前处理软件kubrix

http://www.itascacg.com/software/kubrix




## FLAC 边坡

### 8-1

```
E =10.0e6
poi =0.30
coh =43.0e3
weight =25e3
dila =47.0*dilain1
fri =17.0
ten =0.01e6
grav =-9.8
dens =-weight1/grav0
K=E/(3*(1-2*poi))
G=E/(2*(1+poi))
```

按此输入提示 error bad command()


```
pl set back white
set plot bitmap size (800,510)
plot set window size 37
mainwin size 1 1 position 0 0.8
plot set center 35 0 20
pl set mag 1.10
plot set title text
```

```
pl block group
plot hard 'base' file calculate.bmp
```



### 强度折减塑性区计算命令流



```
ks=1.045
step1=30000
  E1=10.0e6
  poi1=0.30
  coh1=42.0e3/ks
  weight1=25e3
  dila1=0.0
  grav0=-9.8
  dens1=-weight1/grav0
  K1=E1/(3*(1-2*poi1))
  G1=E1/(2*(1+poi1))
command
hist reset
model null
model mohr
pro bulk K1 she G1 dens dens1 coh1 &
friction fri1 dilation dila1 tens ten1
set mech ratio 1e-5
solve step setp1
end command
```