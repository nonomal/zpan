ZPan - Your Last disk on the cloud. 
=========================

[![](https://github.com/saltbo/zpan/workflows/build/badge.svg)](https://github.com/saltbo/zpan/actions?query=workflow%3Abuild)
[![](https://codecov.io/gh/saltbo/zpan/branch/master/graph/badge.svg)](https://codecov.io/gh/saltbo/zpan)
[![](https://wakatime.com/badge/github/saltbo/zpan.svg)](https://wakatime.com/badge/github/saltbo/zpan)
[![](https://api.codacy.com/project/badge/Grade/88817db9b3b04c0293c9d001d574a5ef)](https://app.codacy.com/manual/saltbo/zpan?utm_source=github.com&utm_medium=referral&utm_content=saltbo/zpan&utm_campaign=Badge_Grade_Dashboard)
[![](https://img.shields.io/github/v/release/saltbo/zpan.svg)](https://github.com/saltbo/github.com/saltbo/zpan/releases)
[![](https://img.shields.io/github/license/saltbo/zpan.svg)](https://github.com/saltbo/github.com/saltbo/zpan/blob/master/LICENSE)

![image](https://user-images.githubusercontent.com/17308208/95768427-e93d8080-0ce8-11eb-9371-8752f2b7c91f.png)

## Introduction
ZPan is committed to creating an unlimited speed network disk system, so we use the client to connect directly to cloud storage for design.

Currently ZPan supports all cloud storage platforms compatible with the S3 protocol. You can choose a platform you are familiar with to drive ZPan.

[Online Live](http://zpan.saltbo.cn)(username：demo，password：demo)

## How It Works

ZPan is essentially a URL signature server + a visual file browser.

Because we use a direct-link method for uploading and downloading, in order to ensure the security of uploading and downloading, all URLs used by the client to upload and download must be signed by the server.

Then, in order to conveniently manage the files uploaded by users, we need to develop a visual pseudo file system for file management.

- [saltbo/zpan](https://github.com/saltbo/zpan)
- [saltbo/zpan-front](https://github.com/saltbo/zpan-front)

## Features
- Not limited by server bandwidth
- Support all cloud storage compatible with S3 protocol
- Support file and folder management
- Support file and folder sharing (accessible without logging in)
- Support document preview and audio and video playback
- Support multi-user storage space control
- Support multiple languages

## Why Not ...?

### NextCloud
NextCloud is a very easy to use network disk system. It can be said to be the predecessor in this field. But because it was born relatively early, it was designed base on the local file system. The speed of file transfer is limited by the speed of local network. This means that if you use NextCloud to build a network disk on a server with a bandwidth of one megabyte, the upper bound of the upload and download speed of the network disk is only one megabyte. If you want to increase the speed, you can only upgrade the bandwidth of the server, which is a big cost.

### Cloudreve

Cloudreve is the only product I found before developing ZPan that meets my needs (uploads and downloads are not limited by bandwidth). However, Cloudreve was developed based on PHP at the time, and I was a bit disgusted about that it was troublesome to deploy, so I wanted to implement one by myself in Golang. However, due to some reasons, it was put on hold for more than a year. When I restarted ZPan and it was almost finished, I realized that Cloudreve also used Golang for refactoring during this year.

It is undeniable that Cloudreve has more functions than ZPan does. ZPan will be more restrained in features, as I always believe that more features are not always better. So, if you find that ZPan does not meet your needs, you can also try Cloudreve.

### EyeblueTank

Blue Eye Cloud Disk was also found when I was looking for online storage products in the early days. Generally speaking, it fits my vision and is simple and easy to use. Unfortunately, it also belongs to the traditional network disk. I have communicated with his developers, and they have no plans to support cloud storage.

### Z-File

Z-File is an online file catalog program that supports various object storage and local storage. Its target is to be a commonly used tools by individuals for downloading, or a public file library. It will not be developed in the direction of multiple accounts.

## Contributing
See [CONTRIBUTING](CONTRIBUTING.md) for details on submitting patches and the contribution workflow.

## Contact us
- [Author Blog](https://saltbo.cn).

## Author
- [saltbo](https://github.com/saltbo)

## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsaltbo%2Fzpan.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsaltbo%2Fzpan?ref=badge_large)
