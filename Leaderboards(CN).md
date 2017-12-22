排行榜代表了一个已经达到在某个 stats 上获得“最佳”成绩的玩家的有序列表。 例如，排行榜可能会列出在竞速项目中获得最快时间的玩家们，这样玩家可以与其他玩家比较他们获取的最佳成绩。

Leaderboards 是基于游戏发送给 Xbox Live service 的玩家 stats。 因此，排行榜数据是只读的，您不能直接修改它们。

Xbox Live Unity plugin 提供了一个示例 Leaderboard prefab，您可以使用它来了解如何在您的游戏中实现排行榜。


更多信息, 请参考 [Leaderboards](https://docs.microsoft.com/windows/uwp/xbox-live/leaderboards-and-stats-2017/leaderboards).

## 使用 leaderboard prefabs
Xbox Live Unity plugin包含两个 leaderboard 的 prefab:
* Leaderboard: 表示 leaderboard 的一个 object, 使用了简单的 UI 界面来表示来自 leaderboard 的数据。

* LeaderboardEntry: 一个表示一单行 leaderboard 的 object.

您可以将一个 **Leaderboard** prefab 拖拽进场景. 在 Unity Inspector 中, 您可以设置以下 attributes:

* Stat: 此 leaderboard 相关联的 stat gameobject.
* Leaderboard Type: 结果应该是 leaderboard entries 返回的结果的范围。
* Entry Count:每页显示的数据行数。

您必须构建项目并将其导出到Visual Studio，并使用授权用户登录才能看到真实的数据值。了解更多信息，请看[[Configure Xbox Live in Unity]].


## See also

* [[Configure Xbox Live in Unity]]
* [[Sign into Xbox Live in Unity]]
* [[Stats]]
