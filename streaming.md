# Adding Streaming Services 
This is the process to add popular streaming services to the SteamDeck as non-steam games.  The process works for any stream service that is accessible via chrome on windows PC.

I currently use Disney+, HBOMax, Hulu, Netflix, Paramount+, Prime Video, and YouTube 

## Step-by-Step

### 1. Add Chrome as Non-Steam Game
### 2. Change Parameters
### 3. Add Icons, Banner


/usr/bin/flatpak run --branch=stable --arch=x86_64 --command=/app/bin/chrome --file-forwarding com.google.Chrome @@u %U @@

run --branch=stable --arch=x86_64 --command=/app/bin/chrome --file-forwarding com.google.Chrome @@u @@ --window-size=1024,640 --force-device-scale-factor=1.25 --device-scale-factor=1.25 --kiosk https://www.disneyplus.com
