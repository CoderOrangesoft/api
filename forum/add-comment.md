# 添加回复

> 在相应回帖添加回复  
> `/web/forums/replies/<reply_id>/comments` `POST` `需要cookies`

## POST 请求参数

|    key    |                                              value                                               |  type  |        |
| :-------: | :----------------------------------------------------------------------------------------------: | :----: | :----: |
|  content  |                                      回帖内容（HTML 格式）                                       | string | `必须` |
| parent_id | 回复的其他回复 ID（默认为 0，即直接回复回帖，否则应设置为已有回复的 ID，显示为：“xxx 回复 xxx”） |  int   | `可选` |

## 返回内容

| key |  value  |  type  |
| :-: | :-----: | :----: |
| id  | 回复 ID | string |
