成就是一种全系统的机制，用于在所有的游戏中以一致的方式来引导和奖励用户的游戏内行为。如果您对 Achievements 不太熟悉，请参阅: [Achievements documents](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/achievements-2017/achievements).

从现在开始,所有的新 Title 都会使用 Data Platform 2017 创建在 [Windwos Dev Center](https://dev.windows.com/) .对 achievements 而言, 它的 [Achievements 2017](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/achievements-2017/simplified-achievements) 允许开发者  用 direct calling model 去解锁 新 Xbox Live 的游戏在Xbox One, Windows 10, Windows 10 Phone, Android, and iOS的成就。

关于如何在Dev Center上配置 成就，请参考 [Configure Achievements 2017 on Dev Center](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/achievements-2017/achievements-in-udc).


## 使用脚本

凭借  Achievements 2017，解锁成就或更新进度变得非常简单。这里的关键API是`UpdateAchievementAsync`方法。更多信息，请参阅  [Update_Achievement API](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/achievements-2017/simplified-achievements#updateachievement-api).
在 Unity 中，您可以利用 `AchievementBase` 类。您可以派生这个类，并重载`CalculateProgress`方法来实现您的成就的解锁逻辑。
