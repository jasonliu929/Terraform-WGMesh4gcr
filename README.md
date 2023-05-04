通过Terraform在宁夏、北京区域创建EC2实例，并部署WireGuard服务，以搭建多云云服务器FullMesh网络。主要步骤如下：

1. 配置Credentials用于运行Terraform

export AWS_ACCESS_KEY_ID=AKI....FWL

export AWS_SECRET_ACCESS_KEY=axc.....ay2

2. 修改variables.tf，设置VPC CIDR以及子网CIDR，Key等

3. 修改bootstrap.sh脚本，设置亚马逊云以及其他公有云的云服务器的WireGuard wg0接口IP地址, Endpoint等，然后执行

$ ./bootstrap.sh

4. 运行clean.sh 清理环境

$ ./clean.sh
