# 我的Git学习笔记

 — 郭怀晨馨

## 学习内容的目录

- 什么是Git？有什么特点？
- 学习Git基本流程，使用GitBash完成基本流程
- 使用GitBash推送文档到远程仓库流程
- 替代GitBash提交更方便，更效率的方法
- 学习如何与他人在Github上协作完成项目

## 学习内容

### 一、什么是Git？有什么特点？
- Git --最先进分布式版本控制体系
- 特点：
  - 能够记录每一次文件改动，可随时找到修改的每一个版本
  - 能与多人协作修改，能够合并项目，能清晰看见改动部分

### 二、学习Git基本流程，使用GitBash完成基本流程

- Git基本流程 : clone 、add、commit、push 
- 使用 GitBash 完成基本流程


仓库地址：`https://github.com/Yclsxg/Tasks.git`

```bash
# 克隆远程仓库
git clone https://github.com/Yclsxg/Tasks.git

# 进入仓库目录
cd Yclsxg

# 查看当前目录文件
ls

# 查看当前路径
pwd

# 添加文件到暂存区
git add Yclsxg

# 提交，写提交说明
git commit -m "美化主页 README"

# 推送到远程 main 分支
git push origin main

# 推送到远程 main 分支
git push origin main
```
###  三、使用GitBash推送Hello.md文档到远程仓库流程
- Git 推送流程
1. 初始化本地仓库
   `git init`
   用 `git status` 查看文件状态，此时文件还未被追踪。

2. 添加文件到暂存区
   `git add Hello.md`
   再执行 `git status`，文件变绿，进入暂存。

3. 提交到本地仓库
   `git commit -m "Add the first file"`
   `git status`，提示工作区干净。

4. 绑定远程仓库
   - `git remote -v` 查看远程仓库
   - `git remote add origin 远程仓库地址` 绑定远程仓库

5. 推送到远程仓库
   `git push -u origin master`

### 四、替代 GitBash 提交更方便，更效率的方法
#### VSCode 提交远程仓库方法

##### 操作步骤
1. 打开左侧「源代码管理」面板，查看所有改动文件。
2. 暂存文件：点击加号，可以一次性暂存全部更改，也可以单独暂存某个文件。
3. 提交：填写提交说明，点击对勾提交到本地仓库。
4. 拉取远程更新，保证本地代码最新。
5. 推送到远程仓库，完成上传。

#### VSCode 对比 GitBash
- VSCode：图形界面，鼠标操作，直观看到改动；写代码、文档、提交都在同一个工具内，不容易敲错命令，对新手更友好，日常使用更高效。
- GitBash：依靠输入命令，适合理解 Git 的底层原理，需要记忆大量命令，输错就容易报错。


### 五、学习如何与他人在 Github 上协作完成项目

#### 协作流程
1. **Fork**：复制目标仓库到自己的 GitHub 账号。
2. **Clone**：将 Fork 后的仓库克隆到本地电脑。
3. **新建分支**：为当前任务单独创建分支，不直接在 main 上开发。
4. **修改文件**：编辑、测试内容。
5. **提交并推送到自己的远程仓库**。
6. **创建 Pull Request（PR）**：请求原仓库主人合并改动。
7. **代码评审**：根据别人的反馈修改。
8. **合并**：维护者审核通过，把改动并入原项目。
9. **持续同步**：定期拉取原仓库最新代码，防止冲突。


