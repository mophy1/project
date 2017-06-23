1. 首先到官网上下载最新的版本，下载到本地后赋予可执行的权限。

# chmod +x VMware-Workstation-Full-8.0.0-471780.i386.bundle 
2.执行安装。虽然能够弹出图形的安装界面，但有如下的错误信息。

# ./VMware-Workstation-Full-8.0.0-471780.i386.bundle 
Extracting VMware Installer...done. 
Gtk-Message: Failed to load module "pk-gtk-module": libpk-gtk-module.so: cannot open shared object file: No such file or directory 
Gtk-Message: Failed to load module "canberra-gtk-module": libcanberra-gtk-module.so: cannot open shared object file: No such file or directory 
3.解决上述Gtk的报错，主要是相应的module找不到。

3.1. 先确定需要的module系统是否安装及其位置。

# locate libpk-gtk-module.so 
/usr/lib/gtk-2.0/modules/libpk-gtk-module.so 
# locate libcanberra-gtk-module.so 
/usr/lib/gtk-2.0/modules/libcanberra-gtk-module.so 
3.2.添加系统加载modules的路径。

# vim /etc/ld.so.conf.d/gtk-2.0.conf 
/usr/lib/gtk-2.0/modules 
3.3.重新加载。

# ldconfig 
重新执行安装，然后一路Next就可以了。

./VMware-Workstation-Full-8.0.0-471780.i386.bundle 
Extracting VMware Installer...done. 
注意事项：

locate: can not stat () `/var/lib/mlocate/mlocate.db': No such file or directory

如果出现此错误，请执行updatedb
