# EEG-Fun-Hackz
muselistener.py will let you TYPE BY WINKING.  
1. Connect your Muse to your computer over Bluetooth.  
Download the SDK tools (You need MuseIO and you might need MuseLab and MusePlayer but I don't think so).  
2. run the command   
    muse-io --device Muse-1A2B --osc osc.udp://localhost:5000  
where 1A2B is the ID code of your Muse (its name on your computer as a bluetooth device)  
3. run muselistener.py  
4. put the Muse on your head  
5. follow the instructions to calibrate your passive state, and each of your winks' activity.  
6. wink to type on your computer!!!  

A left wink is read as a 0, and a right wink as a 1.  Each time you wink, you are setting one bit of the letter that you want to write.  
After you've set all 5 bits, the letter will be typed out.  
The mapping of winks to letters is as follows:  
a : 00000  
b : 00001  
c : 00010  
d : 00011  
e : 00100  
f : 00101  
g : 00110  
h : 00111  
i : 01000  
j : 01001  
k : 01010  
l : 01011  
m : 01100  
n : 01101  
o : 01110  
p : 01111  
q : 10000  
r : 10001  
s : 10010  
t : 10011  
u : 10100  
v : 10101  
w : 10110  
x : 10111  
y : 11000  
z : 11001  
backspace: 11111  
anything else maps to the space character.  


For example, if I wink 5 times in the following order: left, left, right, left, left, then I will type the character "e".  

#development  
I made this project with a Muse headset at HackMIT Fall 2015.  This project is not currently in development due to lack of EEG equipment.  Feel free to contribute.
