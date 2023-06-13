# MineCraft-Server
A document for different MineCarft servers.

# Start up
* MAC环境下，安装openjdk20。
```shell
brew install openjdk
echo 'export PATH="/usr/local/opt/openjdk/bin:$PATH"' >> ~/.zshrc
```

* 下载MC服务器[mc-server-1.13.1](https://launcher.mojang.com/v1/objects/fe123682e9cb30031eae351764f653500b7396c9/server.jar)，
* 下载MC服务器[mc-server-1.18.1](https://launcher.mojang.com/v1/objects/125e5adf40c659fd3bce3e66e67a16bb49ecc1b9/server.jar)，

* 启动MC-Server服务

```shell
java -Xms1200m -Xmx1300m -jar server.jar nogui --singleplayer brian
```

在本项目中，可使用
* `sh script/start_1_13.sh`
* `sh script/start_1_18.sh`

>启动过程需要修改eula.txt中变量为true后，重启服务。

启动日志如下：
```python
[21:50:14] [Server thread/INFO]: Starting minecraft server version 1.13.1
[21:50:14] [Server thread/INFO]: Loading properties
[21:50:15] [Server thread/INFO]: Default game type: SURVIVAL
[21:50:15] [Server thread/INFO]: Generating keypair
[21:50:15] [Server thread/INFO]: Starting Minecraft server on *:25565
[21:50:15] [Server thread/INFO]: Using default channel type
[21:50:15] [Server thread/INFO]: Preparing level "world"
[21:50:15] [Server thread/INFO]: Found new data pack vanilla, loading it automatically
[21:50:15] [Server thread/INFO]: Reloading ResourceManager: Default
[21:50:15] [Server thread/INFO]: Loaded 524 recipes
[21:50:16] [Server thread/INFO]: Loaded 571 advancements
[21:50:19] [Server thread/INFO]: Preparing start region for dimension minecraft:overworld
[21:50:20] [Server thread/INFO]: Preparing spawn area: 0%
[21:50:28] [Server thread/INFO]: Time elapsed: 8803 ms
[21:50:28] [Server thread/INFO]: Done (13.488s)! For help, type "help"
```
