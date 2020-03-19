# Geacon

**Implement CobaltStrike's Beacon in Go**

----

*This project is only used for learning protocol analysis and reverse engineering. If someone's rights are violated, contact me to delete the project, and the last DO NOT USE IT ILLEGALLY*



## How to play

1. Setup the teamserver and start a http lisenter, the teamserver will generate the file `.cobaltstrike.beacon_keys`.
2. Compile beacontoo with Jetbrains Idea, use command `java -jar BeaconTool.jar ` to convert java keystore to PEM format.
3. Replace the RSA key pair in the file `cmd/config/config.go` (the RSA private key is not required, I wrote it in the code just for the record)
4. Compile geacon for what platform you want to run, use command `export GOOS="darwin" && export GOARCH="amd64" && go build cmd/main.go`
5. Having fun ! PR and issue is welcome ;)
6. Geacon has just been tested on CobaltStrike 3.14 and only support default c2profile, so many hardcode in the project and I will not try to implement more C2profile support at this moment.



## Protocol analysis

To be continued, I will update as soon as I have time ...


# 盖康


**在Go中实施CobaltStrike的灯塔**

----

*该项目仅用于学习协议分析和逆向工程。如果有人的权利受到侵犯，请与我联系以删除该项目，最后一个请勿非法使用*



## 怎么玩

1. 设置团队服务器并启动http许可，团队服务器将生成文件.cobaltstrike.beacon_keys。
2. 使用Jetbrains Idea编译beacontoo，使用命令java -jar BeaconTool.jar 将Java密钥库转换为PEM格式。
3. 替换文件中的RSA密钥对cmd/config/config.go（不需要RSA私钥，我将其写在代码中只是为了记录）
4. 为您要运行的平台编译geacon，请使用命令 export GOOS="darwin" && export GOARCH="amd64" && go build cmd/main.go
5. 玩得开心 ！公关和问题，欢迎;）
6. eacon刚刚在CobaltStrike 3.14上进行了测试，仅支持默认的c2profile，因此项目中的硬代码如此之多，我现在不尝试实现更多的C2profile支持。



## 协议分析


待续，我将在有时间时更新...


