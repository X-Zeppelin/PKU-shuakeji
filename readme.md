# 北大刷课机

**最后更新于 2020年2月17日**

##基本情况

**运行需求：**Mathematica 11.0+ ，Chrome最新版。（注：Raspberry Pi自带Mathematica，所以可以很方便的在Raspberry Pi上托管！）Mathematica安装请见<u>[这里](https://tiebamma.github.io/InstallTutorial/)</u>.

**基本功能：**自动输入验证码（总体正确率约为93%），自动选课，自动退课（例如如果什么课出现空位，则退掉其它几门课，如果选课失败会立刻尝试补回来。），友善的Mathematica界面。

**实现方法：**以Mathematica为控制/计算平台，通过Chrome Driver托管Google Chrome浏览器实现，所以理论上是和人刷是没有任何区别的（除了刷的频次会高很多）。

**一些细节：**

1. 去年曾尝试过一晚上刷新，没问题的，长时间运行是可靠的。
2. 目前还没听说过谁的课被这个选课机退光了2333（毕竟也没几个人用



**具体初始化的帮助在.nb文件里，请务必读完再跑！！！**



##基本操作 

0. 先激活安装Mathematica/Chrome
1. 打开 **选课机.nb** 文件，依次确认各个事项。
2. 在每次使用前，点击 菜单栏->Evaluation(计算)->Evaluate Initialization Cells(计算初始化单元)
3. 滑到最后，运行代码ShuaKeJi[]。**在这之后你都不应该碰触浏览器！**
4. 你应该马上看见如下界面：

![登录界面](https://i.loli.net/2020/02/17/lAcB5zdrR2DYLJt.png)

5. **一定在右侧Mathematica窗口中输入学号和密码！否则无法在意外退出后恢复！**
6. 点击Login并登录成功后你应该见到Mathematica弹出如下界面：

![选课界面](https://i.loli.net/2020/02/17/HCBkvGpaPwscEVh.png)

7. 选择多门需要的课（注意左上角点击不同页数翻页哦），点击Confirm，并再次点击Correct确认即可。若需要返回请点击右下角的Edit。

   ![确认界面](https://i.loli.net/2020/02/17/GpSY2PlXjsqWoby.png)

8. 确认后即开始刷课，假如你看见Chrome在刷来刷去的话，那就对了！就放手吧！

9. (*高级操作*)自动退课：进入上图界面后，例如我们希望能选上流体力学的话就退掉广相，那么就点击流体力学一栏右侧的Edit键，你应该看见如下界面：

![自动退课](https://i.loli.net/2020/02/17/XpskxzjZydwbEuL.png)

10. 选择广相，并保存。这时候流体力学左侧会出现下拉菜单的按钮，点开你应该可以看到如下的界面。

![确认界面2](https://i.loli.net/2020/02/17/esh2tz14EBnuAlx.png)

11. 如果没问题了，确认好后点击Correct即可。

##免责声明

本程序仅用于学习交流，不建议同学过量使用本刷课机刷课，干扰选课秩序。本人不对该选课机造成的**一切**后果（例如由于使用不当退光了你的课！）担责！！！！

