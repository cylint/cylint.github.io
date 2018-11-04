---
layout: post
title:  "The ITASCA plugin interface. "
tags: flac3d
categories: flac3d
---

* TOC
{:toc}


## The ITASCA plugin interface. 

The Itasca interface allows access to internal data structures and algorithms.

As such it is extremely dangerous – there is no way (even in theory) to prevent the user from writing code that will crash the program, or generate incorrect results.

Access to program data generally starts with the IProgram interface, which can be thought of as the root of a tree of all the interfaces available.

In general program specific data (Flac3D, 3DEC, PFC, etc) will be available in the interface IFLAC3D, which is defined differently for each program.


Itasca接口允许访问内部数据结构和算法。

因此，这是非常危险的 - 没有办法（甚至在理论上），以防止用户编写代码使程序崩溃，或生成不正确的结果。

访问程序数据通常从 IProgram 接口开始，可以被认为是所有可用接口的树的根。

通常，程序特定数据（Flac3D，3DEC，PFC等）将在 IFLAC3D 接口中提供，该接口对每个程序的定义不同。




## Modules
 

Here is a list of all modules:


Utility interface specification  
FISH interface specification  
Kernel interface specification  
Base interface specification  
Utilitysrc  
Example implementation of the IFishLibrary interface  
Module interface specification.  
Constitutive Model interface specification  
FLAC3D 

interface specification 

接口规范

## Namespaces List

Here is a list of all documented namespaces with brief descriptions:


AVector2Util 2D Angular vector class 

dynamic Standardized dynamic library loading routines.
 
itascaxd Itasca Library standard namespace, specific to 2D or 3D 

models The Constitutive Model interface library 


 Constitutive Model 

 本构模型