# daupd
**Docker container Auto UPDate**

This is a simple bash I create to create an extremely simple (and dumb) script that pulls and applies updates to docker container ran with docker-compose. It can also add the scripts to crontab if you want.

>[!IMPORTANT]
>Right now, the script fits exactly my needs, but you are welcome to make adaptations, change, and of course making it better. 

If you want to use the script as is, clone the repo:

```
git clone https://github.com/AlexanderWinters/daupd.git
cd daupd
```

Make sure the `daupd` script is executable:
```
chmod +x daupd
```
And now you can run the script:
```
./daupd
```

If you want to run it from anywhere in CLI, add it to `/usr/local/bin`, or to `$HOME/bin` (you can create the paths if they don't exist). You can also export it to `$PATH`, but I would suggest one of the other solutions so things don't break.


## Future Plans
- Find a way to upload it to package repositories.
- Have the script install itself to `/usr/local/bin` so it always runs from anywhere
- Look into Mac and Windows version (theoretically it should already work on Mac and Windows WSL)
- Allow for other types of containers, not just docker. 
- Maybe dockerize it (doesn't make much sense now)
- More polish
- Maybe GUI