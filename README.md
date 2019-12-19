# 项目名称：博物馆动静皆宜
# Product Requirement（产品说明文档）

| Title                     | Content |
| ------------------------- | ------- |
| Target release(发布日期)  | 2019/11 |
| Epic(史诗名称)            | 博物馆动静导览  |
| Document status(文档状态) | 进行中  |
| Document owner(文件主人)  | 胡凯锋  |
| Designer(领头的设计师)    | 胡凯锋 |
| Developer(领头的开发者)   | 胡凯锋  |
| QA(领头的测试者)          | 胡凯锋  |

- 版本修订记录

|修订版本号|迭代日期|修订内容|迭代者|
|---------|-------|--------|-----|
|v1.0|2019.11.20|文档初稿撰写，建立基本产品文档框架|胡凯锋|
|v1.1|2019.11|-------|胡凯锋|
|v2.0|2019.11|-------|胡凯锋|


- 文档输出环境

|文档名称|版本号|体验环境|撰写时间|撰写人|
|---------|-------|--------|-----|----|
|博物馆动静小程序|v3.1|Andrio10|2019.11.25|胡凯锋|



# Catalogue（目录）
- [Part1 PRD价值主张设计](#价值主张设计)
    - [PRD1加值宣言](#加值宣言)
    - [PRD2核心价值](#核心价值)
    - [PRD3用户痛点](#用户痛点)
    - [PRD4人工智能概率性与用户痛点](#人工智能概率性与用户痛点)
    - [PRD5需求列表与人工智能API加值](#需求列表与人工智能API加值)
- [Part2 原型](#原型)
    - [交互及界面设计](#交互及界面设计)
    - [信息设计](#信息设计)
    - [原型文档](#原型文档)
- [Part3 API产品使用关键AI或机器学习之API的输出入展示](#API产品使用关键AI或机器学习之API的输出入展示)
    - [API使用水平](#使用水平)
    - [API使用比较分析](#使用比较分析)
    - [API使用后风险报告](#使用后风险报告)
    - [API加分项](#加分项)


## 产品定位
兼具参展路线、时间推荐，展品讲解查询的博物馆智能小程序。

## 背景
随着社会的发展和文化知识的普及，每个人都应享有平等的学习知识的权利，基于此，博物馆在对服务残障人士方面需要做出改善变的尤为重要，因此，这款博物馆动静导览小程序为残障人士提供全方位的服务，让残障人士参观博物馆有良好的体验，除此之外，还未多动症小孩提供检测，保护的功能。

## 目标
- 为视觉、听觉、身体等不方便的人士和多动症小孩提供优质的参观服务。

# 价值主张设计

## 加值宣言

- （主要）百度AI的语音合成API对本产品价值部分在于：
    - 通过导览小程序，使用语音合成技术为视觉障碍者提供朗读功能，并可以进行语言选择。残障人士可以通过设置语速、音调、音量等参数，满足个性化需求，为用户带来更好的体验。

- （主要）百度AI的语音识别API对本产品价值部分在于：
    - 通过导览小程序，利用语音识别技术，为听觉障碍者提供声音转成文字的服务。在博物馆讲解员介绍展品的时候，语音识别API可快速准确的将语音转化为文字，方便听觉障碍者使用，能够和普通游客“跟团”参观。

- （辅助）人流量统计API对本产品价值部分在于：
    - 使用人流量统计API，为博物馆进行动态人流量统计，面向馆内、通道等出入口场景，以头肩为识别目标，进行人体检测和追踪，根据目标轨迹判断进出区域方向，实现动态人数统计，返回区域进出人数，进而为用户提供适宜的参观方案。
    

## 核心价值（最小可行性产品）
- 语音合成：能够实现有声读物功能。
- 语音识别：能够准确识别博物馆讲解员的语音介绍转换为文字。
- 人流量统计：动态人流量统计，面向馆内、通道等出入口场景。


## 用户痛点
#### 目标用户
 残障人士；多动症小孩
#### 用户痛点分析

| 角色   | 痛点分析                                                                                                                                                                                                                                                                                                                                                                        |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 身障者 |参观者出行不方便，在参观博物馆时可能由于身体原因无法自己动手使用小程序。                                                                                                                                                                                                                                                                                                                  |
| 视障者 | 参观者在由于视觉障碍无法观看展品，荧幕等。                                                                                                                                                                                                                                                                                                      |
| 聋哑人 | 参观者无法听到讲解员，语音播报等声音；参观者手语博物馆相关工作人员看不懂，引起交流不方便。                                                                                                                                                                                                                                        
|多动症| 在父母未注意到的情况下，多动症小孩到博物馆到处乱窜，触摸甚至破坏展品，造成馆内喧哗。|

## 人工智能概率性与用户痛点
- 语音识别：部分的博物馆讲解员可能是志愿者，未受过专业的培训，在发音的时候不准确的情况下容易导致语音识别及其相关功能的识别结果产生误差。
- 语音合成：在长文字，多音字，方言等合成不准确。

## 需求列表与人工智能API加值

需求列表

| #   | User Story                                                                                                         | Importance | Notes                                   | 技术                |
| --- | ---------------------------------------------------------------------------------------------------- | -------------------- | ---------------------------------------------- | ------------------- |
| 1   | 视觉障碍者不能够看不清/看不见展品，荧幕等，用户需要通过语音了解 | 极其重要             | 核心功能                                       | 百度AI语音合成API   |
| 2   | 听觉障碍者听不清／听不见讲解员（语音播报）的讲解内容，需要通过文字的形式呈现给用户方便了解                     | 极其重要             | 核心功能 | 百度AI语音识别API   |
| 3   | 身体障碍者在出行、参观过程中行动不便，需要为残障人士安排出行、参馆时间路线；需要有人协助残障人士使用博物馆导览小程序                 | 极其重要                 | 核心功能                                       |  百度AI人流量统计API  |
| 4   |     多动症小孩在人多的情况下容易与父母走失，触摸甚至破坏展品，扰乱博物馆秩序，为此需要为这类用户提供特殊的参馆路线          | 重要                 | 核心功能                                       | 百度AI人流量统计API |

## 使用到的API
- 百度API人脸识别
    - [人脸检测](https://ai.baidu.com/docs#/Face-Detect-V3/top)
    - [人脸搜索](https://ai.baidu.com/docs#/Face-Search-V3/top)

- 高德地图API
    - [静态地图](https://lbs.amap.com/api/webservice/guide/api/staticmaps)

# PART2 原型

## 交互及界面设计
## 信息设计
## 原型文档

# PART3 API产品使用关键AI或机器学习之API的输出入展示

## 使用水平 输入+输出
## 使用比较分析
## 使用后风险报告
## 加分项 
## 清单
