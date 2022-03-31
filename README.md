# moonlight-service
systemd service for moonlight

I created this because sometimes moonlight would abruptly quit/abort. If it happens in the middle of playing a game I would have to pause the game and restart moonlight on my raspberry pi. So after doing that a few times I thought it'd be better to automate the process so I created this systemd service which will automatically restart if moonlight exits prematurely. I also included my config file but you should edit it if you choose to use this service. 

Cheers.

NOTE: If anyone wants to know why I created bash scripts(moonrise/moonset) to execute the moonlight commands instead of putting the moonlight commands directly in the service file(in the Exec option) it's because I tried that and it didn't work. I think that moonlight has to be started from bash so that's why I created scripts to start/stop moonlight and it just works this way. Anyways I hope it's useful to someone else besides myself.
