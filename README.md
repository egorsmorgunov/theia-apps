# Theia applications WITH MY EDITIONS in latest tag with root access

[Theia](https://github.com/theia-ide/theia) is a platform to develop Cloud & Desktop IDEs with modern web technologies.

This repository contains example Theia applications based on published Theia extension packages.

- [Theia Docker](#theia-docker)
  - [How to use `zloystrelok/theia` image?](#how-to-use-theiaidetheia-image)
  - [Image Variants](#image-variants)
    - [`zloystrelok/theia:latest`](#theiaidetheialatest)
- [Theia Desktop](#theia-desktop)
- [License](#license)

## Theia Docker

[![dockeri.co](https://dockeri.co/image/zloystrelok/theia)](https://hub.docker.com/r/zloystrelok/theia/)

`zloystrelok/theia` image contains an example of Theia based IDE for Web Developers.

### How to use `zloystrelok/theia` image?

It is recommended to use [`zloystrelok/theia`](#typefoxtheianext) image to have a look at the current state.

This script pulls the image and runs Theia IDE on http://localhost:3000 with the current directory as a workspace.

    docker run -it -p 3000:3000 -v "/www/middlearth:/home/project:cached" zloystrelok/theia

You can pass additional arguments to Theia after the image name, for example to enable debugging:

    docker run -it -p 3000:3000 --expose 9229 -p 9229:9229 -v "/www/middlearth:/home/project:cached" zloystrelok/theia --inspect=0.0.0.0:9229

### Image Variants

#### `zloystrelok/theia:latest`

This image is based on the latest stable released version.

## Theia Desktop

TBD

## License

[Apache 2.0](LICENSE)
