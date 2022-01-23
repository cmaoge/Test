



###

#### 设置YUM源为aliyun

```bash

mv -f /etc/yum.repos.d/CentOS-Base.repo{,.bak_$(date +%F)}
curl -o /etc/yum.repos.d/CentOS-Base.repo https://mirrors.aliyun.com/repo/Centos-7.repo
yum clean all && yum makecache

```