## [KDIFF3](http://kdiff3.sourceforge.net/)

merge发生冲突时，基于控制台的对比往往看起来不是很舒服，所以这时候可视化的对比就比较有意义了，KDIFF3是比较好用的一款。虽然它的界面丑的很。

* 安装

* ```
  brew install Caskroom/cask/kdiff3
  ```

* 配置.gitconfig

* ```
  [merge] 
  tool = kdiff3
  [mergetool]
  keepBackup = false
  [diff]
  tool = kdiff3
  guitool = kdiff3
  [difftool "kdiff3"]
  trustExitCode = false
  ```

* 发生冲突是，使用

* ```
  git mergetool
  ```

* 效果


