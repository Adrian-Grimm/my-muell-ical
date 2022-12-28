# my-muell-ical

[![GitHub](https://img.shields.io/github/v/tag/adrian-grimm/my-muell-ical)](https://github.com/Adrian-Grimm/my-muell-ical)
[![Docker Pulls](https://img.shields.io/docker/pulls/adriangrimm/mymuell.svg?maxAge=604800)](https://hub.docker.com/r/adriangrimm/mymuell)

Creates ical link for My Müll.

Use url http://myserverandport/calendar.ical?city_id=someCityId&area_id=someStreetAreaId with
someCityId and someStreetAreaId to download or subscribe to the calendar.

## someCityId
Can be get via https://mymuell.jumomind.com/mmapp/loxone/lox.php?r=cities

## someStreetAreaId
Can be get via https://mymuell.jumomind.com/mmapp/api.php?r=streets&city_id=someCityId

## create a docker container and execute it by
```sh
sudo docker build . -t my-muell-ical/my-muell-ical
sudo docker run -p 4434:3000 -d my-muell-ical/my-muell-ical
````
