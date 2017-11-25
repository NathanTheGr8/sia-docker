# sia-docker
Docker file taken from https://mtlynch.io/sia-via-docker/

## To Use
Replace "Server Local IP" with your server's lan ip. Note delete the quotes

Replace /storage/sia with your local storage directory

```
sudo docker create \
--name=sia \
--restart=always \
-p "Server Local IP":9985:8000 \
-p 9981:9981 \
-p 9982:9982 \
-v /storage/sia:/mnt/sia \
nathanthegr8/sia-docker
```

Then 
```
sudo docker start sia
```


## Use at your own Risk
I am not sure how much I will be updating this, and I made it for personal use.
