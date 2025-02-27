Meshtastic Map/tile download script
Basics
Download the files in this repo/gist! into a decent folder
Access that folder on a terminal (cmd or powershell should work but haven't tested out of Linux distros)
Create your account at https://www.thunderforest.com/docs/apikeys/ (free or paid, up to you)
Alternatively: can also use https://apidocs.geoapify.com/playground/maps/ (defaults to thunderforest (style atlas))
Validate your account on your email using received validation link.
Log in
Copy API Key from website.
set API key as env var API_KEY
install needed libraries using pip install -r requirements.txt
Execute main script with python main.py
copy downloaded data into folder map at the root of your SD card.
put your sd card into your T-Deck Plus or favourite Meshtastic device that uses Device-UI.
tips and extras
IF IN DOUBT of where data is being written it should be all around the log output but also at the first lines of it.
If you don't like default directory, must use env var DOWNLOAD_DIRECTORY (full path preferably)
set env var DEBUG if you edit this code for it not to download while testing.
Map style can be set in env var MAP_STYLE. Keep in mind if you use same directory as output dir it won't rewrite existing tiles.
