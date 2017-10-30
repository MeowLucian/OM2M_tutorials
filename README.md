# OM2M_tutorials
IOT

## 虛擬環境硬體調整

* CPU core
* Memory
* Bridge network

## Ubuntu 環境調整

* All settings -> Displays -> 1440 x 900

## VMware tools 安裝

將 VMware Tools 10.1.15-6627299.tar.gz 複製到 Desktop

```
cd /home
cd iotclass
cd Desktop
tar zxvf VMware-Tools-10.1.15-6627299.tar.gz
cd vmware-tools-distrib
sudo su -c ./vmware-install.pl
yes
```

## Start OM2M IN-CSE

```
cd org.eclipse.om2m/org.eclipse.om2m.site.in-cse/target/products/in-cse/linux/gtk/x86_64
sh start.sh
```

## Start OM2M MN-CSE

Open new terminal window

```
cd org.eclipse.om2m/org.eclipse.om2m.site.mn-cse/target/products/mn-cse/linux/gtk/x86_64
sh start.sh
```
