### 打包命令  
    .tar  
　　解包：tar xvf FileName.tar  
　　打包：tar cvf FileName.tar DirName  
　　（注：tar是打包，不是压缩！）  
　　.tar.gz 和 .tgz  
　　解压：tar zxvf FileName.tar.gz  
　　压缩：tar zcvf FileName.tar.gz DirName
#### 例子  
    tar -xzvf .tar.gz
      tar [-cxtzjvfpPN] 文件与目录 .... 
      参数： 
      -c ：建立一个压缩文件的参数指令(create 的意思)； 
      -x ：解开一个压缩文件的参数指令！ 
      -t ：查看 tarfile 里面的文件！ 
      特别注意，在参数的下达中， c/x/t 仅能存在一个！不可同时存在！ 
      因为不可能同时压缩与解压缩。 
      -z ：是否同时具有 gzip 的属性？亦即是否需要用 gzip 压缩？ 
      -j ：是否同时具有 bzip2 的属性？亦即是否需要用 bzip2 压缩？ 
      -v ：压缩的过程中显示文件！这个常用，但不建议用在背景搜索执行过程！ 
      -f ：使用档名，请留意，在 f 之后要立即接文档名！不要再加参数！

### 查看linux的版本内核信息  
	1. uname -a  
  Linux node1 3.19.0-59-generic #66-Ubuntu SMP Thu May 12 22:35:27 UTC 2016 x86_64 x86_64 x86_64 GNU/Linux  
	2. cat /proc/version  
	Linux version 3.19.0-59-generic (buildd@lgw01-53) (gcc version 4.9.2 (Ubuntu 4.9.2-10ubuntu13) ) #66-Ubuntu SMP Thu May 12 22:35:27 UTC 2016  
	3. cat /etc/issue  
	Ubuntu 15.04 \n \l   
  4 lsb_release -a  
	No LSB modules are available.  
	Distributor ID:	Ubuntu  
	Description:	Ubuntu 15.04  
	Release:	15.04  
	Codename:	vivid  

### 查看linux磁盘空间大小  
	df -hl  
### 环境变量配置文件  
  ~/.bashrc   
  
  
  


