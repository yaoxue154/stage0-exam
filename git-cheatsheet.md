# diff指令
- `git diff` 查看工作区和暂存区的区别
- `git diff --staged` 查看暂存区和上一次commit的区别
# 后悔两档
- `git restore` 直接将工作区的状态变回仓库【上一次commit】状态，丢失所有修改
- `git restore --staged`将add的内容撤回使得暂存区变回原来的暂存区，工作区修改保留
# 隔离网
- 在根目录下创建.gitignore文件，在文件中输入不需要让git管理的文件和内容，git就不再处理写入的相应内容
- `git status`管理git的状态，功能类似于终端的ls
# git传远程仓库
- `git init`                                 # 初始化仓库（如果还没有）
- `git add .`                                   # 添加所有文件
- `git commit -m "第一次提交"`                    # 提交
- `git remote add origin https://github.com/你的用户名/仓库名.git`   # 关联远程仓库
- `git push -u origin master`                   # 推送到 GitHub
- origin是远程仓库地址的默认别名——它是那串 URL 的代称，不是仓库的名字。起这个名字只是约定俗成，你完全可以改成 upstream 或别的，它指的还是那串地址。
# 终端git commit操作
- `git add . `                          # 把所有修改加入暂存区
- `git commit -m "写清楚你改了什么"`      # 提交
- `git push `                           # 推送到 GitHub
# 修改上一次git的标题
- `git commit --amend -m "新标题"`
# 词源
- diff = difference、restore = re+store 放回存过的状态、amend = 修正、origin = 源头