欢迎来到xbox-live-full-unity-plugin wiki

这个plugin是基于 [xbox-live-unity-plugin](https://github.com/Microsoft/xbox-live-unity-plugin) to support [ID@Xbox](https://www.xbox.com/en-US/developers/id) 项目. 大部分API和都原来保持了一致。

在此 这个plugin中, 我们用 [xbox-live-api](https://github.com/Microsoft/xbox-live-api) 替代了原来的 Xbox Live libraries (e.g. Microsoft.Xbox.Services.UWP.CSharp.dll), 这样一来我们就能够使用成就系统和一些 Xbox Live Creators Program不支持的功能了。但是，由于我们使用 WinRT APIs,所以在 editor 中运行时，会缺少 placeholder.

这个 plugin 仍然在开发中。现在, 它仅仅展示了SignIn以及 Profile, Stats, Leaderboards and Achievements. 开发者们可以通过参考此 plugin 来完成自己的实现.
