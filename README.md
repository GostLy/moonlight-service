# moonlight-service
systemd service for moonlight

I created this because sometimes moonlight would abruptly quit/abort. If it happens in the middle of playing a game I would have to pause the game and restart moonlight on my raspberry pi. So after doing that a few times I thought it'd be better to automate the process so I created this systemd service which will automatically restart if moonlight exits prematurely. I also included my config file but you should edit it if you choose to use this service. Cheers.
