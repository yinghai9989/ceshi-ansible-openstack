
## Links

[Ansible Documentation](http://docs.ansible.com)

[Ansible 笔记](https://wiki.shileizcc.com/display/AN/Ansible)

## 部署计划

初步为三个虚拟机节点，分别为 control0, control1, compute1。

由于集群限制，只能有一个节点可以登录外网，所以这个虚拟机充当 ntp server 和 yum server。

control0 部署 OpenStack 相关的 services，control1 部署中间件和部分OpenStack services，compute1 作为计算节点。