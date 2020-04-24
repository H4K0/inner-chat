# inner-chat
Super simple Debian desktop notify sender

###  For use this script between devices please install libnotify-bin
```
ssh USER@IP_ADDRESS 'DISPLAY=:0 notify-send "MESSAGE"'
```

### libNotify  Resources notes and usage
 SYNOPSIS:
```
  notify-send [OPTIONS] <summary> [body]                     
```
### OPTIONS-> 
```
       -u, --urgency=LEVEL [LEVEL = low, normal, critical]                   
                                                                             
       -t, --expire-time=TIME                                                
              The duration, in milliseconds, for the notification to appear  
                   on screen. (Ubuntu's Notify OSD and GNOME Shell both      
                   ignore this parameter.)                                   
                                                                             
       -i, --icon=ICON[,ICON...]                                             
              Specifies an icon filename or stock icon to display.           
                                                                             
       -c, --category=TYPE[,TYPE...]                                         
              Specifies the notification category. 
```     
### Usage:
## inner-chat [OPTIONS]
```
	Options:
	  -a Direccion del host
	  -u Usuario
	  -t Titulo del mensaje (Entrecomillas si es mas de una palabra)
	  -m Cuerpo del mensaje (Entrecomillas si es mas de una palabra)
	  -i $HOME/icon/ico.ico

	  I.e.:
	     inner-chat -u root -a 192.168.0.2 -t \"Titulo del mensaje\" \
	     -m \"Cuerpo del mensaje\" -i \$HOME/ico.png"
```

# Note:
### Before run the script, please grant privileges:
```
$ chmod u+x inner-chat
```
