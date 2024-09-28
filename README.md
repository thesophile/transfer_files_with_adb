# Transfer files from Phone to PC with Terminal using adb

Install adb
```
sudo apt update
sudo apt install adb
```
Enable developer options in your phone and turn on USB debugging. Connect to your PC and accept the prompt. 

Your device should be listed when:
```
adb devices
```
> [!IMPORTANT]  
> Make sure you have enabled developer options AND turned on USB debugging

Now, you can view the files 
```
adb shell ls /sdcard/
```
Pull the file or directory you want to copy to your PC: 

```
adb pull <file to be copied> <destination>
```
for example:
```
adb pull /sdcard/Download/Telegram
```
