# DGPS
The Construction consists two raspberry pi3s with Aldebaran Modul from Dr.Fasching and Tallysman tw-2410 antenna.The goal is to realize a system with a moving-base and rover. The Base should get its own position without giving basic position coordinates during the moving process. The Rover should get the data from the base and should print the relative distance. 

At this state i have the normal fixed Base, moving Rover solution. 
It´s also not clear why some satellites are chosen and why others are not.I am trying my best
to get to my solution.


To set up my raspberry pi3´s i followed the instructions of:

1.Dr.Fasching: http://drfasching.com/products/gnss/raspignss/installation.html

2. custom-build-robots:https://custom-build-robots.com/raspberry-pi-roboter/praezise-gps-positionierung-rtklib-navigation/7958#comment-1376


On the custom-build-robots the instructor changed the rc.local script on the raspberry pis(rpis) 
which i did not. Instead of changing the rc.local script I wrote:
1.nmeafile.nvs
2.binrfile.nvs
so you easily can switch between those scripts without having a bunch of commands to tap.

I also build the rtklib 2.4.3 on both of my rpis. 

