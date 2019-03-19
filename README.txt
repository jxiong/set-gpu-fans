## BEWARE: THIS PROGRAM WAS MADE TO SET FAN SPEEDS WITHOUT AN ACTIVE X SERVER, SO IF 
## YOU ARE AT DESKTOP THERE ARE MORE CONVENIENT WAYS TO MANAGE TEMPERATURES.

1- Put this entire folder wherever you like (e.g.: /opt/set-gpu-fans);

2- Edit 'cool_gpu' file: change the first line to the directory you choosed;

3- Create a link to 'cool_gpu' in the executable files folder (e.g.: ln
/opt/set-gpu-fans/cool_gpu /usr/local/bin/cool_gpu)

4- Run 'cool_gpu' with a number argument to set this speed (40-100), or with 'stop' to return to 
GPU default state, e.g.:
    cool_gpu 85         set fans to 85%
    cool_gpu stop       stops the program and return GPU to its default state
    cool_gpu            set fan to a temperature dependent value

Details of inner working:
https://sites.google.com/site/akohlmey/random-hacks/nvidia-gpu-coolness#TOC-Faking-a-Head-for-a-Headless-X-Server
