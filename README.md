# ctf01d-automation-training

## Use Docker

### Build docker images with environment

Build environment (change the date)

```
docker build -t sea5kg/ctf01d-automation-training:2026-05-16-build-environment -f Dockerfile.build-environment .
```

Release environment (change the date)

```
docker build -t sea5kg/ctf01d-automation-training:2026-05-16-release-environment -f Dockerfile.release-environment .
```

Build image

```
docker build -t sea5kg/ctf01d-automation-training:2026-05-16 -f Dockerfile .
```

```
docker run --rm -p 10551:10551 -v $PWD/data:$PWD/app/data sea5kg/ctf01d-automation-training:2026-05-16
```

How web will be available on http://localhost:10551/

## Authors

* Evgenii Sopov (mrseakg@gmail.com)
