## 如何
切换存储是很简单的。

1. 第一，运行 `/luckperms export <file>`
2. 接着，完全停止你的服务器
3. 编辑你的配置文件，更改存储类型
4. 开启你的服务器，等待数据存储的初始化
5. 接着，使用 `/luckperms import <file>`
6. 所有的数据已经迁移到新的数据存储中了

<file> 是你想用来存储/加载的文件的名称，文件位于 LuckPerms 的数据文件夹里。你可以任意命名，只要在 import 命令中正确填写。

## 备份
你可以使用这个特性来备份所有你的 LuckPerms 的数据，只需要运行 export 命令，将文件保存到一个安全的地方。

## 这是怎么工作的？
export 命令将所有的数据转换为一串命令，处理后将会重建你的安装，import 命令只是将每个命令运行一遍，这意味着你可以只导出/导入一小部分数据，你删掉不需要的一部分就可以了。