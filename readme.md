You need to create a .env file. I left the commented out options here just as a reminder for me later...

```
PIHOLE_PW=<password>
PIHOLE_ROUTER_IP=<your_router_ip>
PIHOLE_HOST_IP=<your_pihole_ip>
#PIHOLE_NETWORK_DOMAIN=<your.domain.if.you.want>
#PIHOLE_HOST_IPV6
```

You also need to create the folders for the volume mapping. This will help when you upgrade pihole.

```
mkdir etc-dnsmasq.d
mkdir etc-pihole
```

Then,

```
docker compose up -d
```