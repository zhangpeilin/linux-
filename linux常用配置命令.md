## 一、nmcli——网络配置命令

### 显示网卡列表
nmcli connection show

### 显示指定网卡详细信息
nmcli device show enp0s5

### 将指定ip分配给指定网卡
nmcli connection modify <interface_name> ipv4.address  <ip/prefix>
nmcli con mod enp0s5 ipv4.addresses 10.211.55.5/24

### 将指定网关分配给指定网卡
nmcli con mod enp0s5 ipv4.gateway 10.211.55.1

### 将网卡改为手动配置
nmcli con mod enp0s5 ipv4.method manual

### 将DNS分配给网卡
nmcli con mod enp0s5 ipv4.dns 10.211.55.1

### 重启网卡使设置生效
nmcli con up enp0s5

