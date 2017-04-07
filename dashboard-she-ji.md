# 概览（Dashboard）设计

> 理念还是按照五步拆解法，来讲 Dashboard 设计（用户是谁/场景，解决问题/提供价值，分析思路，指标+展示，落地行动）有些特别的点需要注意：

笔者先后负责过三个公司的数据概览页面设计，深刻了解到这个页面的重要性。无论哪一种数据产品，概览（Dashboard）作为用户接触数据的第一个页面，相当于数据产品的门户，担负着提纲挈领，引导分析的重要职能。它有着以下特点

>



## 1. 明确用户和场景

Different users, different data：确认用户角色，并围绕角色设计信息架构和分析框架，参考 [https://medium.com/truth-labs/designing-data-driven-interfaces-a75d62997631](https://medium.com/truth-labs/designing-data-driven-interfaces-a75d62997631)

## 2. 解决问题/提供价值

## 3. 分析思路

## 4. 指标+展示

shape the page，Choose the \*right\* visualizations，default set

1. 帮助用户理解和相信他们看到的数据
   1. 提供上下文信息：提供数据清晰的标题，标签和解释（CEO），或者提供易于理解的指标名称
   2. 使用户相信数据：提供数据的来源，算法以及异常的原因。异常的数据需要提供可验证的途
2. 保持易用性和效果之间的平衡
   1. 尽量避免checkboxes, radio buttons和tab
   2. 首先确定分析的内容和框架，在这个框架提供有限的输入。有限的输入包括时间范围的选择，维度筛选器和计算筛选器（求和/平均/去重）
3. 支持快速的迭代和迅速的反应
   1. 产品响应速度要快，查询快且得到结果
   2. 其中的关键是需要能够对数据进行探索

## 5. 落地行动

This approach resonates with our clients, especially for high-level information.

1. One tactic I've picked up to help with this is to try and use text to communicate exactly what someone wants to know.
2. 数据的呈现最终要落实为可实行的动作

## 6. 设计案例



参照文章和书籍

Dashboard design



