# docker-stunnel
## Usage
### Docker
```
docker run -v ./stunnel.conf:/etc/stunnel/stunnel.conf -p 25:25 bmlandis2010/stunnel
```
### Docker Compose
```
services:
  stunnel:
    container_name: stunnel
    image: bmlandis2010/stunnel
    ports:
      - '25:25'
    volumes:
      - ./stunnel.conf:/etc/stunnel/stunnel.conf
    restart: always
```