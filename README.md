# docker-moinmoin

A moinmoin wiki docker image.

## RUN

```shell
$ docker run -it -d  -p 80:80 \
                    --name=my_wiki \
                    eternnoir/moinmoin
```

super userid: wikiadmin

## Backup

```shell
$ docker cp CONTAINER_ID:/usr/local/share/moin BACKUP_FILE_PATH
```

## Ues Host path

You can use cp first. Then use this command to start moinmoin container.

```shell
docker run -it -d -p 80:80 \
        --name wiki \
        -v MOIN_PATH:/usr/local/share/moin \
        eternnoir/moinmoin

```

## Ref.

Edit from https://github.com/olavgg/moinmoin-wiki
