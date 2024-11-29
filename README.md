# Jenkins-automation-update-script---example
关于jenkins自动化更新镜像的脚本
使用方法：
1. 执行git clone xxxxx.git 拉取到本地
2. 下载jenkins2.480版本镜像
3. 将gitclone下来的jenkins_home挂载到容器内/var/jenkins_home
4. 修改默认路径名称为/var/jenkins_home
5. mv Jenkins-automation-update-script---example /var/jenkins_home
6. 启动命令示例：
7. docker run -d -p 10240:8080 -p 10241:50000 -v /var/jenkins_home:/var/jenkins_home --restart=always --user=root --name jenkins jenkins/jenkins
8. 访问：http://ip:10240
   账号：admin，密码：Gjxx@1q2w3e
