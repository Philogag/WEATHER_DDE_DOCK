# DDE_Dock_Weather
Deepin Linux DDE-Dock weather forcast plugin.  
[Releases](../../releases/)  
install：./install.sh  
uninstall：./uninstall.sh  
## Build

#### Env
`sudo apt-get install -y dde-dock-dev qt5-default libdtkwidget-dev`

#### Build command & Right Output
```
$ qmake weather.pro
Info: creating stash file */Desktop/WEATHER_DDE_DOCK/.qmake.stash
$ make
g++ -c -m64 -pipe -O2 -std=gnu++11 -Wall -W -D_REENTRANT -fPIC -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I. -isystem /usr/include/libdtk-2.0.16/DWidget -isystem /usr/include/libdtk-2.0.16/DCore -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtWidgets -isystem /usr/include/x86_64-linux-gnu/qt5/QtGui -isystem /usr/include/x86_64-linux-gnu/qt5/QtNetwork -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -I. -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -o forcastwidget.o forcastwidget.cpp
/usr/lib/x86_64-linux-gnu/qt5/bin/rcc -name res res.qrc -o qrc_res.cpp
g++ -c -m64 -pipe -O2 -std=gnu++11 -Wall -W -D_REENTRANT -fPIC -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I. -isystem /usr/include/libdtk-2.0.16/DWidget -isystem /usr/include/libdtk-2.0.16/DCore -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtWidgets -isystem /usr/include/x86_64-linux-gnu/qt5/QtGui -isystem /usr/include/x86_64-linux-gnu/qt5/QtNetwork -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -I. -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -o qrc_res.o qrc_res.cpp
/usr/lib/x86_64-linux-gnu/qt5/bin/moc -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -I/home/philogag/Desktop/WEATHER_DDE_DOCK -I/usr/include/libdtk-2.0.16/DWidget -I/usr/include/libdtk-2.0.16/DCore -I/usr/include/x86_64-linux-gnu/qt5 -I/usr/include/x86_64-linux-gnu/qt5/QtWidgets -I/usr/include/x86_64-linux-gnu/qt5/QtGui -I/usr/include/x86_64-linux-gnu/qt5/QtNetwork -I/usr/include/x86_64-linux-gnu/qt5/QtCore -I/usr/include/c++/6 -I/usr/include/x86_64-linux-gnu/c++/6 -I/usr/include/c++/6/backward -I/usr/lib/gcc/x86_64-linux-gnu/6/include -I/usr/local/include -I/usr/lib/gcc/x86_64-linux-gnu/6/include-fixed -I/usr/include/x86_64-linux-gnu -I/usr/include weatherplugin.h -o moc_weatherplugin.cpp
g++ -c -m64 -pipe -O2 -std=gnu++11 -Wall -W -D_REENTRANT -fPIC -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I. -isystem /usr/include/libdtk-2.0.16/DWidget -isystem /usr/include/libdtk-2.0.16/DCore -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtWidgets -isystem /usr/include/x86_64-linux-gnu/qt5/QtGui -isystem /usr/include/x86_64-linux-gnu/qt5/QtNetwork -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -I. -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -o moc_weatherplugin.o moc_weatherplugin.cpp
/usr/lib/x86_64-linux-gnu/qt5/bin/moc -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -I/home/philogag/Desktop/WEATHER_DDE_DOCK -I/usr/include/libdtk-2.0.16/DWidget -I/usr/include/libdtk-2.0.16/DCore -I/usr/include/x86_64-linux-gnu/qt5 -I/usr/include/x86_64-linux-gnu/qt5/QtWidgets -I/usr/include/x86_64-linux-gnu/qt5/QtGui -I/usr/include/x86_64-linux-gnu/qt5/QtNetwork -I/usr/include/x86_64-linux-gnu/qt5/QtCore -I/usr/include/c++/6 -I/usr/include/x86_64-linux-gnu/c++/6 -I/usr/include/c++/6/backward -I/usr/lib/gcc/x86_64-linux-gnu/6/include -I/usr/local/include -I/usr/lib/gcc/x86_64-linux-gnu/6/include-fixed -I/usr/include/x86_64-linux-gnu -I/usr/include weatherwidget.h -o moc_weatherwidget.cpp
g++ -c -m64 -pipe -O2 -std=gnu++11 -Wall -W -D_REENTRANT -fPIC -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I. -isystem /usr/include/libdtk-2.0.16/DWidget -isystem /usr/include/libdtk-2.0.16/DCore -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtWidgets -isystem /usr/include/x86_64-linux-gnu/qt5/QtGui -isystem /usr/include/x86_64-linux-gnu/qt5/QtNetwork -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -I. -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -o moc_weatherwidget.o moc_weatherwidget.cpp
/usr/lib/x86_64-linux-gnu/qt5/bin/moc -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -I/home/philogag/Desktop/WEATHER_DDE_DOCK -I/usr/include/libdtk-2.0.16/DWidget -I/usr/include/libdtk-2.0.16/DCore -I/usr/include/x86_64-linux-gnu/qt5 -I/usr/include/x86_64-linux-gnu/qt5/QtWidgets -I/usr/include/x86_64-linux-gnu/qt5/QtGui -I/usr/include/x86_64-linux-gnu/qt5/QtNetwork -I/usr/include/x86_64-linux-gnu/qt5/QtCore -I/usr/include/c++/6 -I/usr/include/x86_64-linux-gnu/c++/6 -I/usr/include/c++/6/backward -I/usr/lib/gcc/x86_64-linux-gnu/6/include -I/usr/local/include -I/usr/lib/gcc/x86_64-linux-gnu/6/include-fixed -I/usr/include/x86_64-linux-gnu -I/usr/include forcastwidget.h -o moc_forcastwidget.cpp
g++ -c -m64 -pipe -O2 -std=gnu++11 -Wall -W -D_REENTRANT -fPIC -DQT_NO_DEBUG -DQT_PLUGIN -DQT_WIDGETS_LIB -DQT_GUI_LIB -DQT_NETWORK_LIB -DQT_CORE_LIB -I. -isystem /usr/include/libdtk-2.0.16/DWidget -isystem /usr/include/libdtk-2.0.16/DCore -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtWidgets -isystem /usr/include/x86_64-linux-gnu/qt5/QtGui -isystem /usr/include/x86_64-linux-gnu/qt5/QtNetwork -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -I. -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -o moc_forcastwidget.o moc_forcastwidget.cpp
rm -f libHTYWeather.so
g++ -m64 -Wl,-O1 -shared -o libHTYWeather.so weatherplugin.o weatherwidget.o forcastwidget.o qrc_res.o moc_weatherplugin.o moc_weatherwidget.o moc_forcastwidget.o  -L/usr/X11R6/lib64 -ldtkwidget -ldtkcore -lQt5Widgets -lQt5Gui -lQt5Network -lQt5Core -lGL -lpthread
```

![alt](preview.png)  
![alt](FashionMode.png)  

## Icon Name Rule

| Weather | Day | Night | Image |
| :-----: | :-: | :---: | :---: |
| Clear | 01d.png | 01n.png | ![alt](icon/Default/01d.png) |
| Clouds | 02d.png | 02n.png | ![alt](icon/Default/02d.png) |
| Clouds | 04d.png | 04n.png | ![alt](icon/Default/03d.png) |
| Clouds | 04d.png | 04n.png | ![alt](icon/Default/04d.png) |
| Rain | 09d.png | 09n.png | ![alt](icon/Default/09d.png) |
| Rain | 10d.png | 10n.png | ![alt](icon/Default/10d.png) |
| Thunder | 11d.png | 11n.png | ![alt](icon/Default/11d.png) |
| Snow | 13d.png | 13n.png| ![alt](icon/Default/13d.png) |
| Fog | 50d.png | 50n.png | ![alt](icon/Default/50d.png) |
| NA | na.png | na.png | ![alt](icon/Default/na.png) |

#### Because the night time is not very accurate, we use the same icon for day and night.

## Change log
### 5.4 (2019-03-03)
Add temperature unit set:  
![alt](TemperatureUnit.png)
![alt](Fahrenheit.png)
### 5.3 (2019-01-07)
* Support icon theme  
![alt](IconTheme.png)

### 5.0 (2018-12-19)
* Change API to https://openweathermap.org to support world wide weather forcast.
