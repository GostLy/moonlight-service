# moonlight-service
systemd service for moonlight

I created this because sometimes moonlight would abruptly quit/abort. If it happens in the middle of playing a game I would have to pause the game and restart moonlight on my raspberry pi. So after doing that a few times I thought it'd be better to automate the process so I created this systemd service which will automatically restart if moonlight exits prematurely. 

I also included my moonlight config file but you should edit it if you choose to use it and if not then you should edit "moonrise" to change the location of the config file. If you do choose to use/edit my config file then I'll explain a few settings I use; In my config file "app = Desktop" refers to an game/app shortcut that I added to the Geforce Experience under "Shield" settings on my Host PC. So "Desktop" points to "C:\Windows\System32\mstsc.exe" which just tells moonlight to stream the full desktop so I recommend adding that if you haven't already. I also have "viewonly = true" because I have my controller connected(wirelessly) to my Host PC so I didn't need/want any input being sent to my raspberry pi. The rest of the settings should be self-explanatory.

Cheers.

NOTE: If anyone wants to know why I created bash scripts(moonrise/moonset) to execute the moonlight commands instead of putting the moonlight commands directly in the service file(in the Exec option) it's because I tried that and it didn't work. I think that moonlight has to be started from bash so that's why I created scripts to start/stop moonlight and it just works this way. Anyways I hope it's useful to someone else besides myself.
