# WififPassCheck
Don't fret about asking for the password of a previously connected network that slipped your mind. With just your Laptop and these straightforward steps, you can effortlessly retrieve the password in four simple stages.

1. Open Cmd
   
2. Type down this command - 'netsh wlan show profile' (without the ' ' quotation mark)
   It shows you all the Previous Networks your device was connected to. Somethinging like this.
<img width="292" alt="image" src="https://github.com/devkothaaari/WififPassCheck/assets/107349582/739cc954-4ccc-4167-88eb-e04e9481a0ce">

3. Now type - netsh wlan export profile folder=C:\ key=clear
    (Executing this command will save an XML file containing the KeyMaterial of all previously password-protected networks to your C drive.)
   
4. Go to Windows (C:) on File Explorer, in the bottom you will find all the extracted files, Open these files using Notepad. U will get all the deets like
  SSIDConfig, connectionType, connectionMode, keyMaterial.
<img width="132" alt="image" src="https://github.com/devkothaaari/WififPassCheck/assets/107349582/4d41cc9f-48ce-4aae-8119-a2c40ef83d03">

6. Within the Keymaterial tab, you will discover the password that was utilized to protect the network.
   <img width="388" alt="image" src="https://github.com/devkothaaari/WififPassCheck/assets/107349582/9ab7926c-5895-4e83-8a2f-cdc98a4ebe41">
   
  
