# 标签的基本操作

标签命令

|                命令                 |               描述               |
| :---------------------------------: | :------------------------------: |
|          git tag tag_name           |     新建标签，默认标签为HEAD     |
|    git tag -a tag_name -m 'xxx'     |    添加便签并设置标签描述信息    |
|               git tag               |           查看所有标签           |
|         git tag -d tag_name         |         删除一个本地标签         |
|      git push origin tag_name       |        推送本地标签到远程        |
|       git push origin --tags        | 推送全部未推送过的本地标签到远程 |
| git push origin :refs/tags/tag_name |         删除一个远程标签         |