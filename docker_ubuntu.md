docker容器

Ubuntu环境安装

启动容器

docker run -ti --rm -p 5901:5901 -p 222:22 -v D:\wl\docker\data:/data  ubuntu-python-vnc 

vim安装

sudo apt-get install vim-gtk 

```
容器配置修改：
	vncserver:
		/usr/bin/vncserver
		
			$geometry = "1920x1080";
			
	pip安装
			wget https://bootstrap.pypa.io/get-pip.py
			python get-pip.py 
        修改源
        	~/.pip/pip.conf 
                    [global]
                    index-url = https://mirrors.aliyun.com/pypi/simple/ 
           
	python3安装
			
			apt-get install python3-dev

		pip3 install virtualenv
		
		设置python3虚拟环境：
			cd /data/venv/py3/
			virtualenv -p python3 dev
		进入python3虚拟环境：
			source dev/bin/activate
	
	git安装
			sudo apt-get install git
	
	安装中文字体
    
    	apt-get install -y fonts-droid-fallback ttf-wqy-zenhei ttf-wqy-microhei fonts-arphic-ukai fonts-arphic-uming
			
```

​	启动pycharm

​			cd  /data/ide/pycharm-2017.2.3/bin

​			sh pycharm.sh

​	激活码 

​		 http://xidea.online

​		 http://idea.liyang.io 

​	安装redis客户端

​		apt-get install redis-tools