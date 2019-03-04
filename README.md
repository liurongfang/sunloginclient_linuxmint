I just modify **scripts/common.sh**,make it work in Linux Mint,

others please see [sunlogin office website](https://sunlogin.oray.com/zh_CN/download).

following is original information.

-
Sunlogin Client for linux Version 9.6.1.13983



Function introduction:
  When you use this version of Sunlogin Client for linux you have 
	1)Remote desktop		:You can control this computer by another operating platform(a computer, intelligent mobile phone or a pad)
	2)Remote file management	:You can manage this computer's file system and transfer file with another operating platform(a computer, intelligent mobile phone or a pad)
	3)ssh				:You can use this computer's ssh service by another operating platform(a computer, intelligent mobile phone or a pad) 
	4)Wake up function		:You can wake up or shut down this machine by Sunlogin Remote if you have a wake-up stick
	5)VPN 			        :You can connect with other computers within a VPN net




How to use:
  When you get the package of Sunlogin Client for linux Version 9.6.1.13983 named sunloginclient_packet.tar.gz (or some other name), input
		
		tar xf sunloginclient_linux.tar.gz
		cd sunloginclient

  1)Green version:
    Then you can find a shell script file named run.sh , if you just want to use the Remote desktop function and do not want to install it, just run this script
		
		./run.sh
	
    If you system have installed firefox , it will automatically pop up firefox browser interface and the address is http://xxx.xxx.xxx.xxx:30080/ (xxx.xxx.xxx.xxx is your computer's ipv4 address), You can find the Quick Code and Security Code ,you can use Quick Code and Security Code to control this computer by another operating platform(a computer, intelligent mobile phone or a pad).

  2)Installed version:
    If you to install this version of Sunlogin Client for linux , input the following content as root

		./install.sh
    
    If you want to uninstall it you can go the path you installed in (/usr/local/sunlogin) and into the scripts path

		cd /usr/local/sunlogin

    Or just at the current path above , input the following content as root

		./uninstall.sh

    When you have installed this version of Sunlogin Client , you want to start it , input the following content as root

		./start.sh

    If you want to stop it , input the following content as root

		./stop.sh


    When you start an installed Sunlogin Client , you can enter http://xxx.xxx.xxx.xxx:30080 ( xxx.xxx.xxx.xxx is your computer's ipv4 address or 127.0.0.1 ) in your browser and then do some operation (such as login logout or change settings)



Note:
    1) You'd better close your system's firewall if you want have a better use of the functions on Sunlogin Client
    2) You should make your system's firewall allow other computer to access 30080 port(TCP), if you want do operations in other computer(unless you close you firewall)
    3) You should make your system's firewall allow other computer to access Wakeup port(UDP) you have set , if you want to use wake up function(unless you close you firewall)
    4) You should make your system's firewall allow other computer to access LAN discovery port(UDP) you have set , if you want to direct connected by Sunlogin Remote within same LAN(unless you close you firewall)



Copyright(C) 2009-2018 Oray-All Rights Reserved.
www.sunlogin.com
