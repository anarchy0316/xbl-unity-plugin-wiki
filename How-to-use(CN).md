* 如果您的title是在 [Windows Dev Center (UDC)](http://dev.windows.com/)上创建的, 那么无论你是在使用 Xbox Live Creators Program 或是 ID@Xbox,  你都可以按照[Configure Xbox Live In Unity](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/get-started-with-creators/configure-xbox-live-in-unity)使用本 plugin.
更多信息请参考 [Develop in Unity](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/get-started-with-creators/develop-creators-title-with-unity).

* 如果您的title是在  [Xbox Developer Portal (XDP)](https://xdp.xboxlive.com/)上创建的, 那么您不能使用Xbox LiveAssociation Wizard。哎导入 Unity插 件后，请按以下步骤操作:
  1. __Build the project__
      1. 通过选择  __File > Build Settings__ 或者按下 __Ctrl+Shift+B__ 打开 __Build Settings__ 窗口。
      2. 确保你有你想要测试的场景包含在 __Scenes In Build__ 中。如果它不在，请打开该 Scene 并选择 __Add Open Scenes__.
      3. 在 __Platform__ 下选择 __Universal Windows Platform__ 并点击 __Switch Platform__ 切换到 __Univesrsal Windows Platform__。
		(如果是 Unity 5.x, 切换到 __Windows Store__ 平台，选择 __Platform__ 下的 __Windows Store__，然后点击 __Switch Platform__ ，然后将 __SDK__ 设置为 __Universal 10__)
      4. 勾上 __Unity C# Projects__，以启用 script debugging .
      5. 点击__Build__并指定项目的位置。     
  2. [__将您的Visual Studio项目与您的UWP应用程序关联__](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/get-started-with-partner/get-started-with-visual-studio-and-uwp#3-associate-your-visual-studio-project-with-your-uwp-app)
  在 Visual Studio 中打开生成的UWP项目，然后右键单击 Visual Studio 中的项目，然后选择 __Store > Associate App with the Store__.
  3. [__将Xbox Live配置添加到UWP应用程序__](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/get-started-with-partner/get-started-with-visual-studio-and-uwp#4-associate-your-visual-studio-project-with-your-xbox-live-enabled-title)
  4. [__将Internet功能添加到您的Visual Studio项目中__](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/get-started-with-partner/get-started-with-visual-studio-and-uwp#6-add-internet-capabilities-to-your-visual-studio-project)
  5. [__更改目标设备的sandbox__](https://docs.microsoft.com/en-us/windows/uwp/xbox-live/xbox-live-sandboxes#switch-your-pcs-development-sandbox)
  6. __编译并运行Visual Studio中的UWP应用程序__
