[Link to Blog](http://yetanotherpointlesstechblog.blogspot.com/2016/04/emulating-bluetooth-keyboard-with.html)


After follow the instruction in the blog, reboot the Pi

1. plug a keyboard to the Pi

2. terminal 1: 

    ```
    sudo /etc/init.d/bluetooth stop
    
    sudo /usr/sbin/bluetoothd --nodetach --debug -p time
    
    ```
   terminal 2:
   
   ```
   sudo hciconfig hcio 
   
   sudo hciconfig hcio up
   
   sudo python btk_server.py
   
   ```
   connect pi with teh iPhone (paired)
   
   terminal 3:
   
   ```
   sudo python kb_client.py
   ```
   
   check the iPhone and type on the keyboard
   
   
   
   
