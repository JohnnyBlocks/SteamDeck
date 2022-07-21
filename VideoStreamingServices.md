# Video Streaming Services
This is the process to add popular streaming services to the SteamDeck as non-steam games.  The process works for any stream service that is accessible via chrome on windows PC.  It will create a dedicated shortcut that can be run as a steam game, allowing you to stream content full screen.

I currently use Disney+, HBOMax, Hulu, Netflix, Paramount+, Prime Video, and YouTube
<img src="media/add_nonsteam_header.jpg" alt="drawing" width="75%"/>  
## Step-by-Step

### Prerequisite
Decide which streaming service you want to add.  Find the URL for the streaming section.  
This is the URL you are on once successfully logged in and ready to make a video selection.  
For this demonstration I will be adding Disney+.  
The URL is https://www.disneyplus.com.

### A. Add Chrome as Non-Steam Game  
1.  Restart into '**Desktop**' Mode of the Deck.

2.  Start '**Steam**' so it runs in Desktop mode.

3.  In Steam, click the '**ADD A GAME**' button in the lower left corner.  
<img src="media/add_nonsteam_1.png" alt="drawing" width="75%"/>  

4.  Select '**Google Chrome**' from the list and click '**ADD SELECTED PROGRAMS**'

5.  '**Google Chrome**' should now show in your list of game.  
    <img src="media/add_nonsteam_2.png" alt="drawing" width="75%"/>  

### B. Change Name and Parameters
6.  Right click on '**Google Chrome**' in your game list and select '**Properties...**'  
    The properties for the shortcut will open.
    <img src="media/add_nonsteam_3.png" alt="drawing" width="75%"/>

7.  Click into the area that says '**Google Chrome**' and change the name.  
    I am adding Disney Plus, so I changed the name to 'Disney+'

8.  Ignore '**TARGET**' and '**START IN**' fields.

9.  Replace the '**LAUNCH OPTIONS**' with this entire code segment, replacing the disneyplus URL with the streaming service of your choice.  
```
    run --branch=stable --arch=x86_64 --command=/app/bin/chrome --file-forwarding com.google.Chrome @@u @@ --window-size=1024,640 --force-device-scale-factor=1.25 --device-scale-factor=1.25 --force-dark-mode --enable-features=WebUIDarkMode --kiosk https://www.disneyplus.com
    ```    
10.  Click in the Dark Square next to '**Disney+**' and change it to a Disney+ image file of your choice then close the '**SHORTCUT**' window.  
    <img src="media/add_nonsteam_4.png" alt="drawing" width="75%"/>
15. Disney+ is now in your game library as a non-steam game.  
    Restart into '**Game Mode**'

### C. Add Controller Layout, Grid Icons, Banner, and Heroes
<img src="media/add_nonsteam_5.jpg" alt="drawing" width="75%"/>  

11. Find '**Disney+**' in your game library and click on it to select it.

12. Click on the controller icon 🎮 to the right to add a controller layout.  
    The '**Disney+ Controller Settings**' window will open.
    <img src="media/add_nonsteam_7.jpg" alt="drawing" width="75%"/>  


13. Select the Controller Layout that is ideal for you.  
    The default '**Web Browser**' makes the controller work intuitively with the streaming services.  
    You can customize it to your liking or search for a community configuration of your choice.  
    There is a '**Disney+ for SteamDeck**' controller configuration that I am using.
    
12. Add Icon, Banner, and Heroes for Disney+ to make it look like an offical app.
<img src="media/add_nonsteam_6.jpg" alt="drawing" width="75%"/>    

    This can be done via [SteamGridDB](https://www.steamgriddb.com/) manually, via the [SGDBoop](https://www.steamgriddb.com/boop) app, or via [BoilR](https://github.com/PhilipK/BoilR)     
    This site will have guides linked here once I have time to write them up.
