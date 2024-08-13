---
title: 让 KDE 可以像 GNOME 一样使用 Meta 键进行后台窗口调度
tags:
---
众所周知，KDE Plasma 的 Meta 键也就是 Win 键或者叫 Super 键是很难直接在图形界面的设置里面直接重新调度 Remap,当你尝试要单独去映射 Meta 键的时候总会乱码，所以需要借助命令行的作用来使得 Meta 键位失效或者 Remap
1. 原来的 Meta 键是唤起 KDE 的菜单，要想使得它失效，可以应用以下命令：
   `kwriteconfig5 --file kwinrc --group ModifierOnlyShortcuts --key Meta ""`
2. 如果要将 Meta 映射为激活后台切换调度，也就是图形界面设置里面 KWin 的"Overview=Meta+W,Meta+W,显示/隐藏桌面总览"，要使用如下命令：
   首先是映射：
   `kwriteconfig5 --file kwinrc --group ModifierOnlyShortcuts --key Meta "org.kde.kglobalaccel,/component/kwin,,invokeShortcut,Overview"`
3. 然后是重启 KWin ：
   `qdbus org.kde.KWin /KWin reconfigure`

找到解决办法的 Reddit 讨论链接：
https://www.reddit.com/r/kde/comments/t416lu/rebind_meta_key_to_open_overview/

来源：[让 KDE 可以像 GNOME 一样使用 Meta 键进行后台窗口调度](https://hcy-asleep.github.io/%E8%AE%A9-KDE-%E5%8F%AF%E4%BB%A5%E5%83%8F-GNOME-%E4%B8%80%E6%A0%B7%E4%BD%BF%E7%94%A8-Meta-%E9%94%AE%E8%BF%9B%E8%A1%8C%E5%90%8E%E5%8F%B0%E7%AA%97%E5%8F%A3%E8%B0%83%E5%BA%A6/)