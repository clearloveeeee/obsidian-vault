### 添加网卡驱动程序
1.将ethernet文件夹添加
	包含以太网驱动初始化，和MAC的驱动程序
	ethernet_init 初始化以太网的引脚和设置以太网中断的优先级
	ethernet_read_phy 和 ethernet_write_phy 这两个函数，这两个函数用来 读取和配置 PHY 芯片内部寄存器的
	ethernet_chip_get_speed 函数用来获取网络的速度和双工状态
2.添加以太网驱动文件
	打开stm32f4xx_hal_conf.h文件，使能HAL_ETH_MODULE_ENABLED以太网模块
	添加ETHERNET peripheral configuration 、PHY configuration section、Common PHY Registers、Extended PHY Registers
### lwip配置
1.添加lwip src文件
	src_api->api
	src_core->core下除ipv6
	src_netif->netif路径下ethernet.c文件
	arch通过ST官方lwIP和正点官方例程
2. lwipcommon.c设置ip、mac、子网掩码等内容
