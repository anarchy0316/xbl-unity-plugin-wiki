Stats 是您想要追踪玩家的关键信息。您使用Xbox Live跟踪的 Stats 应该是与玩家相关的Stats，并以某种方式显示。 存在有两种 stats，featured stats 和 normal stats. 有关更多信息，请参阅 [Player Stats](https://docs.microsoft.com/windows/uwp/xbox-live/leaderboards-and-stats-2017/player-stats).


## Featured stats
Featured stats 是在开发中心定义的。 他们会出现在你的 title 的 Game Hub 中。 这些将使您的游戏中心看起来更有趣，并生成自动排行榜以保持玩家的参与度。 你也可以使用它们来引起对你游戏中某些游戏机制的关注，因为这些对于 Xbox Live上的所有玩家都是可见的，即使他们不拥有你的title.

> Note: 开发人员中心上配置的所有统计数据均为 featured stats. Featured stats 和 leaderboards 是要同时配置的。 每个 leaderboards 都基于一个 stats。 每个 featured stats 都会有一个相关的全球排行榜。

从现在开始, 在 [Windwos Dev Center](https://dev.windows.com/) 上创建的所有的新 titles 都将使用 Data Platform 2017. 关于如何配置相关，请参阅 [Configuring Featured Stats or Leaderboards on Dev Center with Data Platform 2017](https://docs.microsoft.com/windows/uwp/xbox-live/leaderboards-and-stats-2017/player-stats-configure-2017)

## Normal stats
其他的 stats 会被当作 normal stats.他们不需要在 Dev Center上配置。你可以通过 `StatisticManager.SetStatisticNumberData`, `StatisticManager.SetStatisticIntegerData` or `StatisticManager.SetStatisticStringData` method 去设置或更新它们。关于更多信息,详见 see [Updating Stats 2017](https://docs.microsoft.com/windows/uwp/xbox-live/leaderboards-and-stats-2017/player-stats-updating).

## 使用 stat prefabs
通过使用Xbox Live Unity插件，您可以轻松地Unity项目中添加在并显示 stats。 与登录步骤类似，您可以选择使用提供的的prefab，或将提供的脚本附加到您自己的自定义 gameobject 中。

更多相关信息，详见[Using the player stat prefabs](https://docs.microsoft.com/windows/uwp/xbox-live/get-started-with-creators/add-stats-and-leaderboards-in-unity#using-the-player-stat-prefabs).

> Note: 如果你没有为 stats 设置任何 value,当你调用 `StatisticManager.GetStatistic`时 会发生 " Stat not found in document"的错误。所以当您在 Unity 中添加了一个具有您 featured stats 正确 ID 的 stats prefab后，仍然有可能发生 "Stat not found in document" 的错误。你可以选择在最一开始设置这个value然后重试。


## See also

* [[Configure Xbox Live in Unity]]
* [[Sign into Xbox Live in Unity]]
