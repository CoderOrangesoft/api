# 作品列表

> 获取任意用户最新作品的信息  
> `/creation-tools/v1/user/center/work-list` `GET`

## URL 参数

|   key   |    value     | type |        |
| :-----: | :----------: | :--: | :----: |
| user_id |   用户 ID    | int  | `必须` |
| offset  |     页码     | int  | `必须` |
|  limit  | 每一页的数量 | int  | `必须` |

## 返回内容

|   key   |                      value                       | type |
| :-----: | :----------------------------------------------: | :--: |
|  items  | 由多个 JSON 构成的作品列表（[查看详情](#items)） | list |
| offset  |                       页码                       | int  |
|  limit  |                   每一页的数量                   | int  |
|  total  |                  该用户作品总数                  | int  |
| counted |                      `未知`                      | bool |

### items

|      key      |                      value                       |  type  |
| :-----------: | :----------------------------------------------: | :----: |
|      id       |                     作品 ID                      |  int   |
|     type      |                       类型                       |  int   |
|   work_name   |                      作品名                      | string |
|    preview    |                   封面图片链接                   | string |
|  view_times   |                    被浏览次数                    |  int   |
| collect_times |                    被收藏次数                    |  int   |
|  liked_times  |                    被点赞次数                    |  int   |
|   parent_id   |            原创：0；再创作：原作品 ID            |  int   |
|  fork_enable  |                  是否允许再创作                  |  bool  |
|  fork_times   |                   被再创作次数                   |  int   |
| publish_time  |                  作品发布时间戳                  |  int   |
|  description  |                     作品介绍                     | string |
|     role      | 在作品创作中的角色（此处似乎只可能为`"AUTHOR"`） | string |
| is_coll_work  |                  是否为协作作品                  |  bool  |
