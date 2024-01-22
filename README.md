# MystHeliumSensecapm1
Combined Mysterium node and Helium miner for Seeed Sensecap m1 &; crankk 
Combined Mysterium node and Helium miner for Seeed Sensecap m1 , for installation using Balena cloud fleet install and using Balena Cli to push install to your own fleets.  This combines repos from nebra for sensecapm1 firmware and balena-myst repo making one docker compose file. this can also be used alongside Crankk and install crank using the ssh method adding your ssh key to the config.json of you balena install found on your sd card .  
 find balena cloud : 
https://dashboard.balena-cloud.com/login
find balena cli :
https://github.com/balena-io/balena-cli

google how to install there is lots of youtube vidios to show you

you may need to add your key to 
https://dashboard.balena-cloud.com/preferences/sshkeys
and install on fleets in develper mode if you want to add crankk to your mining setup too  as ssh might be disabled in production mode

please note no code has been changed form the original repos used folders have been combined and a new docker-compose yml made i take no credit for the code.

If you require crankk too install to your device using balena cli and the docker compose file found hear and then follow the senscapm1 ssh install method from [the ](https://crankk.io/guides/)https://crankk.io/guides/.

if you dont want crankk you dont need to add any ssh keys .

config.json should look like this just add "os":{"sshKeys":["ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDA8YtPDCUXwfLqa9I1QjEg0QLbqqyiCVafflU8Nh6ngjCuxdhY/1O8EbV6HP8B1U3N8xobimRJ2gzhqhSqQCUFvzl2ruh2rP87rkyP1hC8FqQqQC0taXHdimKem6Mqo6myxXAliJVwgXo19laKKgVNwx2oqsSGyFHgaLJgoS0CXyIa/dAzm0KT94plX7w/e0OitPtSbmk8rgj0A8SjUSAuWZiJHhfQKAsY50HycCc/6Whfp4Tj8xEZBdhcloAt+QumzbHgaoNlecicMNbKr9gq3CO9tTc4VsRacAt6QWLH4aPCXwjI+rYswOydLGAB3aclkS9phuGUFz9XbEar73wnVgCCzCbNbPGXtZBFdnefYWORhhPBXHXK5RFHws1flDWVV1dzPg8PtVwc+LMESE+THZUWakubviQySbUtuKlW6EgxiM= oliver@DESKTOP-2KPAE4O"]}

replacing the example key with your key.  the top section will be in the file already as is installed when you flash your sd 


{"apiEndpoint":"https://api.balena-cloud.com","appUpdatePollInterval":900000,"applicationId":"21597","deltaEndpoint":"https://delta.balena-cloud.com","developmentMode":"true","deviceApiKey":"4224de9015d0473","deviceApiKeys":{"api.balena-cloud.com":"4224de901b5548fd0473"},"deviceType":"raspberrypi4-64","listenPort":"48484","logsEndpoint":"https://logs.balena-cloud.com","mixpanelToken":"9ef939ea64cb6cd8bbc96af72345d70d","registryEndpoint":"registry2.balena-cloud.com","userId":"229348","vpnEndpoint":"cloudlink.balena-cloud.com","vpnPort":"443","uuid":"0045545447b52f879543","registered_at":174590839,"deviceId":12317,"hostname":"nebra-55DFB1.local","os":{"sshKeys":["ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDA8YtPDCUXwfLqa9I1QjEg0QLbqqyiCVafflU8Nh6ngjCuxdhY/1O8EbV6HP8B1U3N8xobimRJ2gzhqhSqQCUFvzl2ruh2rP87rkyP1hC8FqQqQC0taXHdimKem6Mqo6myxXAliJVwgXo19laKKgVNwx2oqsSGyFHgaLJgoS0CXyIa/dAzm0KT94plX7w/e0OitPtSbmk8rgj0A8SjUSAuWZiJHhfQKAsY50HycCc/6Whfp4Tj8xEZBdhcloAt+QumzbHgaoNlecicMNbKr9gq3CO9tTc4VsRacAt6QWLH4aPCXwjI+rYswOydLGAB3aclkS9phuGUFz9XbEar73wnVgCCzCbNbPGXtZBFdnefYWORhhPBXHXK5RFHws1flDWVV1dzPg8PtVwc+LMESE+THZUWakubviQySbUtuKlW6EgxiM= oliver@DESKTOP-2KPAE4O"]}}


Claim myst node as per myst instructions on their site ie local ip of the device plus :4449 port in brouser 
please note helium devices should be already onboarded so device is alraedy on their blockchain . 
