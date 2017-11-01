# OM2M_tutorials
OM2M tools for IOT(Internet Of Things).

This example is using OM2M to implement getting the phone's gps and transmitting to server.

![OM2M_01](images/OM2M_01.PNG?raw=true)

--------------------------

## Virtual Environment Hardware setting

Open VMware as administer

* CPU core
* Memory
* Bridge network

![bridge_01](images/bridge_01.png?raw=true)

Edit -> Virtual Network Editor

![bridge_02](images/bridge_02.png?raw=true)

## Ubuntu OS setting

* All settings -> Displays -> 1440 x 900

--------------------------

## VMware tools installation

Copy `VMware Tools 10.1.15-6627299.tar.gz` to Desktop

```
cd /home
cd iotclass
cd Desktop
tar zxvf VMware-Tools-10.1.15-6627299.tar.gz
cd vmware-tools-distrib
sudo su -c ./vmware-install.pl
yes
```

--------------------------

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

## OM2M Resource Tree Tool

http://localhost:8080/webpage

> username: admin
>
> password: admin

![webpage_01](images/webpage_01.png?raw=true)

![webpage_02](images/webpage_02.png?raw=true)

## Start Node-red

Open new terminal window

```
sudo node-red
```
> password: iotclass

http://127.0.0.1:1880/

* Grid

![setting_01](images/setting_01.png?raw=true)

* MN-CSE Flow

![node_red_01](images/node_red_01.png?raw=true)

* IN-CSE Flow

![node_red_02](images/node_red_02.png?raw=true)

* Export

![setting_02](images/setting_02.png?raw=true)

* Deploy MN-CSE

![webpage_03](images/webpage_03.png?raw=true)

* Deploy IN-CSE

![webpage_04](images/webpage_04.png?raw=true)

* Postman Post

![postman_01](images/postman_01.png?raw=true)

![webpage_05](images/webpage_05.png?raw=true)

* Web locations check

http://localhost:1880/locations

![locations_check](images/locations_check.png?raw=true)

* Xml file check

![xml_check](images/xml_check.png?raw=true)