### 配置步骤
1.将ethernet文件夹添加
	包含以太网驱动初始化，和MAC的驱动程序
	ethernet_init 初始化以太网的引脚和设置以太网中断的优先级
	ethernet_chip_get_speed 函数用来获取网络的速度和双工状态