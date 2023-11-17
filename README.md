# Node-ws说明
用于node环境的玩具和容器，基于node三方ws库，集成哪吒探针服务，可自行添加环境变量
* PaaS 平台设置的环境变量
  | 变量名        | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | UUID         | 否 |0dc5f3c0-002b-420e-86ef-7a779dfc9101|
  | PORT         | 否 |  3000  |  监听端口                    |
  | TIME         | 否 |2 * 60 * 1000| 保活间隔时间，默认2分钟  |
  | URL          | 否 |https://www.google.com| 保活的域名，不填写不开启| 
  | NEZHA_SERVER | 否 |        |哪吒客户端域名                |
  | NEZHA_PORT   | 否 | 5555   |当哪吒端口为443时，自动开启tls，无需设置TLS变量| 
  | NEZHA_KEY    | 否 |        | 哪吒探针客户端专用 Key        |
  | NAME         | 否 |        | 节点名称前缀，例如：Serv00    |
  | DOMAIN       | 是 |        | 项目分配的域名或已反代的域名，不包括https://前缀  |

* 本项目已编译自访问功能，如需要，在index.js第二行中添加项目分配的域名，第三行为访问周期，根据需要修改。
* 域名/sub查看节点信息，也是订阅地址，包含https://或http://前缀，非标端口，域名:端口/sub
    
* 温馨提示：对于风控比较严格的平台建议修改完变量后，混肴后再部署，能够避免被封号，绝对安全，READAME.md为说明文件，请不要上传。
js混肴地址：https://obfuscator.io 全部使用默认配置就好，
* 如需进一步修改，右边的Releases中有未混淆的源代码
