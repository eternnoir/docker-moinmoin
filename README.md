# docker-moinmoin

A moinmoin wiki docker image.

## RUN

```shell
$ docker run -it -d  -p 80:80 \
                    -v /opt/moin/data:/usr/local/share/moin/data \
                    --name=my_wiki \
                    eternnoir/moinmoin
```

## Ref.

Edit from https://github.com/olavgg/moinmoin-wiki
