һ���������裺
	1����bmpproject�ļ����е�images�ļ��������е�ͼƬ���ص�GEC6818�����壨Cortex-A52��ϵͳ��/root/bmp/�С�
		cd /root/
		ls
		mkdir bmp�����û�оʹ�����
		cd bmp
		ls
		��tftp�����ļ�������tftp ����Windowsϵͳ����IP -g -r �����ļ���
		
	2����Ubuntu12.04ϵͳ�н������show_bmp.c�� main.c��init.c�ļ�������armbmp�ļ���
			 arm-linux-gcc *.c -o armbmp 

	3����armbmp�ļ����ص�GEC6818�����壨Cortex-A52��ϵͳ��/root/bmp/�С�
			rx ���ص��ļ���
			rz -y
			tftp ����Windowsϵͳ����IP -g -r �����ļ�

	4���޸�armbmp�ļ�Ȩ�ޡ�
			chmod 777 armbmp

	5��ִ��armbmp�ļ���
			./armbmp


	
	


	