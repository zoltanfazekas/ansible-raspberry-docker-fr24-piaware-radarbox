# ansible-raspberry-docker-fr24-piaware-radarbox
Ansible playbook for installing Docker and deploying Dockerized Flightradar24, Piaware, and Radarbox applications on Raspberry Pi

You can specify the following variables in this playbook or define them in a separate file:

$HOST: you can define your host in a separate ansible host file, or provide the IP address

$USER: your username on Raspberry

$FR24KEY: you can find your FR24 sharing key here: https://www.flightradar24.com/account/data-sharing

$PIAWARE_ID: you can find your Flightaware unique identifier here: https://www.flightaware.com/adsb/stats/user/

$LAT: Decimal latitude
$LON: Decimal longitude
$ALT: Altitude above MSL in meters
Get your exact coordinates and altitude above sealevel in meters from one these websites:
https://www.freemaptools.com/elevation-finder.htm
https://www.mapcoordinates.net/en

$RADARBOX_KEY: start the fr24feed-piaware docker container, then issue the following command and it will show your Radarbox sharing key: docker exec <CONTAINER ID> rbfeeder --showkey --no-start
