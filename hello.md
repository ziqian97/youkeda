#绑定本地仓库到github

##进入正确的文件夹路径
假设本地已经有叫youkeda的文件夹，用cd命令进入youkeda这个文件夹

##初始化为git仓库
用git init 命令将一个文件夹初始化为一个git仓库（如果初始化错误，比如初始化youkeda这个仓库，却不小心将他的上级文件夹app初始化为git仓库，就要删除app文件夹下的.git文件（这是一个隐藏文件，用ls -a查询可见）删除命令rm -rf .git  。 删除后进入youkeda文件夹，重新初始化

##绑定远程仓库
用git remote -v命令查询当前git仓库是否绑定远程仓库，显示空白，则没有绑定
绑定远程仓库命令：git remote add origin 仓库地址
绑定成功之后，可用git remote -v查询，完成后就已经绑定好了
如果绑定错误，可执行git remote remove origin来移除绑定
