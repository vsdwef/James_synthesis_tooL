## 工具名称：James_synthesis_tooL

研发目的：旨在帮助技术人员在日常渗透测试或攻防演练中对于漏洞及指纹的积累，形成自己强大的漏洞库及指纹库。相比于nuclei脚本可能会相对无脑简化！且采用GUI设置，使用起来也更加方便！

1、指纹管理

![James_synthesis_tool md631515 6786314](https://github.com/user-attachments/assets/aa25ceca-6942-44fa-a2d2-94d20cf499a3)


2、漏洞管理
![James_synthesis_tool md631563 7714092](https://github.com/user-attachments/assets/85af9de0-75b4-4366-a5d9-f3c984e308d7)


对于POST 请求的漏洞，无论请求体是什么类型，直接从burpsuite中复制到请求体中，相比于编写 nuclei poc。这个会无脑一些！
![James_synthesis_tool md632134 4902264](https://github.com/user-attachments/assets/d44b13c3-1c9d-4ebb-93de-bc59a1b8e405)


3、指纹识别
![image](https://github.com/user-attachments/assets/4f87e130-2b7a-4acd-ac90-34663126cb27)



4、漏洞识别
![image](https://github.com/user-attachments/assets/f56380a8-cb3f-406f-a3a2-0bf5d6ada0e9)



5、联动指纹识别-漏洞自动攻击
![image](https://github.com/user-attachments/assets/e3448be2-4854-47af-99cc-53983a205a21)




6、配置页面
![image](https://github.com/user-attachments/assets/4c5d5dcb-2353-42b4-9a7b-c22283a01c69)



7、启动工具
Win系统，双击James_synthesis_tool.bat
![image](https://github.com/user-attachments/assets/25eb83bd-545e-4ee4-b1d5-28bf4bac15d7)

Mac 
::当前处于 jdk8 启动命令

java -javaagent:James_synthesis_tool.jar  -Dfile.encoding=utf-8 -jar James_synthesis_tool.jar

::当前jdk 版本>11 启动命令

java -javaagent:James_synthesis_tool.jar --module-path ./lib --add-modules javafx.controls,javafx.fxml -jar -Dfile.encoding=utf-8 -jar James_synthesis_tool.jar



PS：工具正常使用是基于jdk 8（经测试jdk > 11 不再内置javafx）
如果发现打不开工具可以下载lib文件放于图示位置，启动命令修改为：
java -javaagent:James_synthesis_tool.jar --module-path ./lib --add-modules javafx.controls,javafx.fxml -jar -Dfile.encoding=utf-8 -jar James_synthesis_tool.jar
![image](https://github.com/user-attachments/assets/708b9d55-9401-4d6e-b6e4-d8b1dc9b9a6a)


其他疑问：可联系作者

![James_synthesis_tool md631436 4842084](https://github.com/user-attachments/assets/dcdeb86e-e8b4-4439-956c-0e9a4e8f8e45)

James安全团队

![image](https://github.com/user-attachments/assets/d7ab9c0b-94d3-406f-992f-2662d27be49a)

欢迎加群交流
![04d7d1426f6aa76b68ba03511dfb2e5](https://github.com/user-attachments/assets/0074c8b0-a1cf-46ca-bb7c-b67c4f82169d)
