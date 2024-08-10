一、操作步骤：
	1）将bmpproject文件夹中的images文件夹中所有的图片下载到GEC6818开发板（Cortex-A52）系统的/root/bmp/中。
		cd /root/
		ls
		mkdir bmp（如果没有就创建）
		cd bmp
		ls
		（tftp下载文件）：（tftp 电脑Windows系统网口IP -g -r 下载文件）
		
	2）在Ubuntu12.04系统中交叉编译show_bmp.c、 main.c、init.c文件，生成armbmp文件。
			 arm-linux-gcc *.c -o armbmp 

	3）将armbmp文件下载到GEC6818开发板（Cortex-A52）系统的/root/bmp/中。
			rx 下载的文件名
			rz -y
			tftp 电脑Windows系统网口IP -g -r 下载文件

	4）修改armbmp文件权限。
			chmod 777 armbmp

	5）执行armbmp文件。
			./armbmp


	
	


	