# 在 Debian Linux 上安装 PPMessage

> 假设你已经安装了Debian Linux 8.4的操作系统，并且已经通过Github clone了PPMessage的源代码。

```bash
# git clone https://github.com/PPMESSAGE/ppmessage.git
# cd ppmessage

```

> 以下文档中都假设你现在处于这个ppmessage目录之下，确认在这个目录中，你能看到dist.sh这样的文件。所有的操作都以root身份运行。对于类似AWS的虚拟机没有提供root，只能通过sudo来提升到root权限，如果在部署上出现问题可以联系我们，针对PPMessage我们提供付费的部署和开发培训服务。

```bash
# ls
LICENSE    README.md  dist.sh*   ppmessage/

```

> 执行 deploy-ppmesage-on-linux.sh 这个脚本能够帮助你在 Linux 上安装 PPMessage 所依赖的 Debian 包和 Python 的开发包以及一些必须通过下载源码进行手动编译的过程。

```bash
# sh ppmessage/depoly/deploy-ppmesage-on-linux.sh

```

> 执行 dist.sh，这个脚本能够帮助你创建数据库和NGINX的配置文件，安装 PPMessage 所需要的 node 的工具和开发包，以及打包、发布、启动、停止 PPMessage 的应用。

```bash
# sh dist.sh bootstrap
# sh dist.sh bower
# sh dist.sh npm
# sh dist.sh gulp
# sh dist.sh start

```



