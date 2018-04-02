# DGPS
The construction consists two raspberry pis, model 3 with an Aldebaran Modul from Dr.Fasching and each a Tallysman tw-2410 antenna.The goal is to realize a system with a moving-base and a rover modul with RTKLIB. The Base should get its own position via GPS without giving position coordinates during or before the moving process. The Rover should get the data from the base modul and print the relative distance. 

At this state i have the normal fixed-base, moving-rover solution. 
It´s also not clear why some satellites are chosen from the system/rtklib and why others are not, although i receive good signals.
The data transfer is realized in nvs binr mode, just look at the sketch in this file-ordner.

To set up my raspberry pi3´s i followed the instructions of:

1.Dr.Fasching: 
http://drfasching.com/products/gnss/raspignss/installation.html and 

2. custom-build-robots:
https://custom-build-robots.com/raspberry-pi-roboter/praezise-gps-positionierung-rtklib-navigation/7958#comment-1376


On the custom-build-robots the instructor changed the rc.local script on the raspberry pi(rpis) 
which i did not. Instead of changing the rc.local script I wrote:
1.nmeafile.nvs
2.binrfile.nvs
so you easily can switch between those scripts without having a bunch of commands to tap.

I also build the rtklib 2.4.3 on both of my rpis. Like i mentioned before at the moment i still stuck with the fixed-base, moving-roving solution, trying to realize the moving-base, moving-rover solution.  

