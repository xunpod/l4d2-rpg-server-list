# 更新地址

鉴于某些服务器的IP会动态变化，本项目将每周更新一次，通常在周五晚上。

获取地址1：https://docs.qq.com/doc/DQnlEZWNjUE13aWlI

获取地址2：[Release](https://github.com/yxnan/block-l4d2-rpg-servers/releases/latest/download/rpglist.json)

# 屏蔽方法

### Windows

获取上述的`rpglist.json`，导入火绒或者其他类似能提供IP过滤名单的软件即可


### Linux

运行：

```bash
sudo ./iptables-import.sh rpglist.json   # 换成你下载的实际路径
```

OK，现在列表中的RPG服就被全部屏蔽了，你将不会在游戏中任何地方看到它们。

## 如果你想自行生成屏蔽列表，参考下列步骤

1. 取得 SteamWebAPI key (https://steamcommunity.com/dev/apikey)

2. 运行 `build-rpglist.sh YOUR_API_KEY_HERE`

3. 当前目录下将生成一个 `rpglist.json`，即最终结果
