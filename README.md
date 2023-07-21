# Codemao API

> 编程猫社区 API 文档

## 概述

Codemao API 项目由[Coderorangesoft](https://shequ.codemao.cn/user/2557945)发起，基于 codemao-team-api，旨在弥补codemao-team-api的不足

## 特征

- 易于学习，解释清晰，小白也可以快速上手
- 更新速度快，随时适配接口的最新状态
- ......

## 约定

1. 在每个 API 头部，会有类似这样的介绍：

   > 修改用户密码  
   > `/tiger/v3/web/accounts/password` `PATCH` `需要cookies`

   !> 注意

   - 没有特殊标注的 API 都基于这个 URL：`https://api.codemao.cn`
   - URL 中类似这样的表达`/abc/<user_id>`，`<xxx>`是一个变量，一般不会说明变量含义，可以从`<user_id>`看出是用户 ID
   - 大部分 API 介绍出于隐私等原因，不提供请求示例，请自行尝试
   - 如果请求不需要用到 cookie，不会专门标注

2. API 中的`返回内容`栏目表现的是请求成功的理想状态
3. `10|[5,200]`中 10 表示默认值为 10，`|`后面为取值范围（区间表示，取整数），此处最小为 5，最大为 200

## 加入我们

如果你想参与本文档的编写与维护，并且符合以下要求，请[发送邮件到 orangesoft@111.com](mailto:orangesoft@111.com) ，并附上你的信息
| 信息 | 重要程度 |
|:----:| :-------:|
|github|    必要   |
| mail |    必要   |
|  qq  | 选择性需要 |

### 要求
- 用编程猫账号，且对编程猫社区的功能有基本了解
- 有 Github 账号，会使用 Github 进行协作开发
- 有基本的网络通信知识
- 有团队合作意识

> 查看[贡献指南](/CONTRIBUTING.md)

## 问题反馈

尽管我们尽力做到最好，但仍然存在许多有待改进之处：

- 许多地方标注了`未知`
- 仍然处于编写过程中，并不包含全部 API
- 文档本身可能存在一些错误

您的任何宝贵意见都可以通过[邮件（orangesoft@111.com）](mailto:orangesoft@111.com)反馈，如果您会使用 Git，可以直接向本文档代码仓库发送 pull 请求（快捷操作：点击文档顶部的编辑文档链接）。
