# Jenkins-automation-update-script---example
关于jenkins自动化更新镜像的脚本
使用方法：
1. 执行git clone https://github.com/StarryGalaxyX/Jenkins-automation-update-script---example.git 拉取到本地
2. 下载jenkins2.480版本镜像
3. 将gitclone下来的jenkins_home移动到：/var/jenkins_home
4. mv Jenkins-automation-update-script---example/jenkins_home /var/jenkins_home
5. 启动命令示例：
6. docker run -d -p 10240:8080 -p 10241:50000 -v /var/jenkins_home:/var/jenkins_home --restart=always --user=root --name jenkins jenkins/jenkins
7. 访问：http://ip:10240
   账号：admin，密码：Gjxx@1q2w3e
