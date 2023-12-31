# 关注列表

> 获取任意用户所关注的用户  
> `/creation-tools/v1/user/followers` `GET`

## URL 参数

|   key   |    value     | type |        |
| :-----: | :----------: | :--: | :----: |
| user_id |   用户 ID    | int  | `必须` |
| offset  |     页码     | int  | `必须` |
|  limit  | 每一页的数量 | int  | `必须` |

## 返回内容

|   key   |                      value                       | type |
| :-----: | :----------------------------------------------: | :--: |
|  items  | 由多个 JSON 构成的用户列表（[查看详情](#items)） | list |
| offset  |                       页码                       | int  |
|  limit  |                   每一页的数量                   | int  |
|  total  |                     作品总数                     | int  |
| counted |                      `未知`                      | bool |

### items

|     key     |     value      |  type  |
| :---------: | :------------: | :----: |
|     id      |    用户 ID     |  int   |
|  nickname   |    用户昵称    | string |
| avatar_url  |  用户头像链接  | string |
|   n_works   |   用户作品数   |  int   |
| total_likes | 用户被点赞总数 |  int   |
| is_followed | 是否关注该用户 |  bool  |
| description |  用户自我描述  | string |
