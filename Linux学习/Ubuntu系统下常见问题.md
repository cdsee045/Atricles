###无法连接github
通过修改hosts文件实现直连
1. 在[ip查询](https://www.ipaddress.com) https://www.ipaddress.com 查询 github.com ， github.global.ssl.fastly.net， assets-cdn.github.com
 和 codeload.github.com 网址对应的ip
1. Ctrl + Alt +T 打开terminate输入以下代码打开hosts文件
    `
    sudo gedit /etc/hosts
    `
2. 将记录的IP及对应的网址添加到hosts文件中，如图

3. 重启网络服务，在终端输入以下命令
    `
    /etc/init.d/network-manager restart

    `
4. 可以用 Ping github.com 测试下是否可以连接



###