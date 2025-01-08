**node output:**
![node output](https://github.com/user-attachments/assets/5c76cb5b-1763-49c9-a5bd-b65cbb522485)


**nignix output:**
![nignix output](https://github.com/user-attachments/assets/01142afe-d306-4ae2-a7bd-0713251f818b)

```C:\Users\adity>docker --version
Docker version 27.3.1, build ce12230

C:\Users\adity>docker info
Client:
 Version:    27.3.1
 Context:    desktop-linux
 Debug Mode: false
 Plugins:
  ai: Ask Gordon - Docker Agent (Docker Inc.)
    Version:  v0.1.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-ai.exe
  buildx: Docker Buildx (Docker Inc.)
    Version:  v0.18.0-desktop.2
    Path:     C:\Program Files\Docker\cli-plugins\docker-buildx.exe
  compose: Docker Compose (Docker Inc.)
    Version:  v2.30.3-desktop.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-compose.exe
  debug: Get a shell into any image or container (Docker Inc.)
    Version:  0.0.37
    Path:     C:\Program Files\Docker\cli-plugins\docker-debug.exe
  desktop: Docker Desktop commands (Alpha) (Docker Inc.)
    Version:  v0.0.15
    Path:     C:\Program Files\Docker\cli-plugins\docker-desktop.exe
  dev: Docker Dev Environments (Docker Inc.)
    Version:  v0.1.2
    Path:     C:\Program Files\Docker\cli-plugins\docker-dev.exe
  extension: Manages Docker extensions (Docker Inc.)
    Version:  v0.2.27
    Path:     C:\Program Files\Docker\cli-plugins\docker-extension.exe
  feedback: Provide feedback, right in your terminal! (Docker Inc.)
    Version:  v1.0.5
    Path:     C:\Program Files\Docker\cli-plugins\docker-feedback.exe
  init: Creates Docker-related starter files for your project (Docker Inc.)
    Version:  v1.4.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-init.exe
  sbom: View the packaged-based Software Bill Of Materials (SBOM) for an image (Anchore Inc.)
    Version:  0.6.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-sbom.exe
  scout: Docker Scout (Docker Inc.)
    Version:  v1.15.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-scout.exe
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


PS E:\wisdom\docker1\niginx ex> docker build -t my-nginx .
[+] Building 46.1s (8/8) FINISHED                                                                  docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                               0.3s
 => => transferring dockerfile: 121B                                                                               0.0s
 => [internal] load metadata for docker.io/library/nginx:latest                                                    3.9s
 => [auth] library/nginx:pull token for registry-1.docker.io                                                       0.0s
 => [internal] load .dockerignore                                                                                  0.1s
 => => transferring context: 2B                                                                                    0.0s
 => [internal] load build context                                                                                  0.2s
 => => transferring context: 604B                                                                                  0.0s
 => [1/2] FROM docker.io/library/nginx:latest@sha256:42e917aaa1b5bb40dd0f6f7f4f857490ac7747d7ef73b391c774a41a8b9  39.3s
 => => resolve docker.io/library/nginx:latest@sha256:42e917aaa1b5bb40dd0f6f7f4f857490ac7747d7ef73b391c774a41a8b99  0.1s
 => => sha256:c44f27309ea1a5e557aff07fbd5ece457d5cb85583f795b34f342d5550a08a5c 1.40kB / 1.40kB                     0.3s
 => => sha256:da8cc133ff821c8b0ac7a6667e3a2e70ee6eb04f850e38088f59720017a869db 1.21kB / 1.21kB                     0.5s
 => => sha256:1e109dd2a0d75eb2ab2491daec5b300e99027ffdd528998612b693f3347b97e4 405B / 405B                         0.7s
 => => sha256:bd98674871f548eff8a4e4f3d4aa1ba504320ccbabfb0a217c4ea5c23b6144fd 957B / 957B                         0.8s
 => => sha256:2b99b9c5d9e5679c839357944d083c55c4c045e2cae21f84dfcfe5841e2ea59b 627B / 627B                         0.6s
 => => sha256:566e42bcee1cd697dcab6098c082789af33bc8cbcbaa95c8adbad87283c85c75 43.84MB / 43.84MB                  36.4s
 => => sha256:fd674058ff8f8cfa7fb8a20c006fc0128541cbbad7f7f7f28df570d08f9e4d92 28.23MB / 28.23MB                  22.8s
 => => extracting sha256:fd674058ff8f8cfa7fb8a20c006fc0128541cbbad7f7f7f28df570d08f9e4d92                          2.7s
 => => extracting sha256:566e42bcee1cd697dcab6098c082789af33bc8cbcbaa95c8adbad87283c85c75                          1.3s
 => => extracting sha256:2b99b9c5d9e5679c839357944d083c55c4c045e2cae21f84dfcfe5841e2ea59b                          0.1s
 => => extracting sha256:bd98674871f548eff8a4e4f3d4aa1ba504320ccbabfb0a217c4ea5c23b6144fd                          0.1s
 => => extracting sha256:1e109dd2a0d75eb2ab2491daec5b300e99027ffdd528998612b693f3347b97e4                          0.1s
 => => extracting sha256:da8cc133ff821c8b0ac7a6667e3a2e70ee6eb04f850e38088f59720017a869db                          0.1s
 => => extracting sha256:c44f27309ea1a5e557aff07fbd5ece457d5cb85583f795b34f342d5550a08a5c                          0.1s
 => [2/2] COPY index.html /usr/share/nginx/html/index.html                                                         1.1s
 => exporting to image                                                                                             0.9s
 => => exporting layers                                                                                            0.5s
 => => exporting manifest sha256:cbf76a0d49748f2f69fdea782ab8de995dcae4e906a654c13c6d6f79474acb87                  0.0s
 => => exporting config sha256:2efe65667d65155fb349fdd427b0d2305a8f528091da71a3d43cbe34bacdf33d                    0.0s
 => => exporting attestation manifest sha256:6033a099ad01333a3090437084408d52c5ef733ec189a7ee9176bf2d66752751      0.1s
 => => exporting manifest list sha256:e76f8d48b9714fb18ffaddcd4da0ad0a97511846ac07d450f15ce0968675ba26             0.1s
 => => naming to docker.io/library/my-nginx:latest                                                                 0.0s
 => => unpacking to docker.io/library/my-nginx:latest                                                              0.1s

View build details: docker-desktop://dashboard/build/desktop-linux/desktop-linux/7vdy4a57xcj83khiysbb8j7ku
PS E:\wisdom\docker1\niginx ex> docker run -d -p 8080:80 my-nginx
248b49a40d053fc2f6a48ac80786d2cf0d962c35bf117b987cdb42f3780a296e
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
PS E:\wisdom\docker1\niginx ex> docker ps
CONTAINER ID   IMAGE      COMMAND                  CREATED         STATUS         PORTS                  NAMES
248b49a40d05   my-nginx   "/docker-entrypoint.…"   2 minutes ago   Up 2 minutes   0.0.0.0:8080->80/tcp   intelligent_jang
PS E:\wisdom\docker1\niginx ex> docker stop 248b49a40d05
248b49a40d05
PS E:\wisdom\docker1\niginx ex> docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

PS E:\wisdom\docker1\niginx ex> docker pull alpine
Using default tag: latest
latest: Pulling from library/alpine
38a8310d387e: Download complete
Digest: sha256:21dc6063fd678b478f57c0e13f47560d0ea4eeba26dfc947b2a4f81f686b9f45
Status: Downloaded newer image for alpine:latest
docker.io/library/alpine:latest
PS E:\wisdom\docker1\niginx ex> docker inspect alpine
[
    {
        "Id": "sha256:21dc6063fd678b478f57c0e13f47560d0ea4eeba26dfc947b2a4f81f686b9f45",
        "RepoTags": [
            "alpine:latest"
        ],
        "RepoDigests": [
            "alpine@sha256:21dc6063fd678b478f57c0e13f47560d0ea4eeba26dfc947b2a4f81f686b9f45"
        ],
        "Parent": "",
        "Comment": "buildkit.dockerfile.v0",
        "Created": "2024-12-05T12:49:04Z",
        "DockerVersion": "27.3.1",
        "Author": "",
        "Config": {
            "Hostname": "",
            "Domainname": "",
            "User": "",
            "AttachStdin": false,
            "AttachStdout": false,
            "AttachStderr": false,
            "Tty": false,
            "OpenStdin": false,
            "StdinOnce": false,
            "Env": [
                "PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin"
            ],
            "Cmd": [
                "/bin/sh"
            ],
            "Image": "",
            "Volumes": null,
            "WorkingDir": "/",
            "Entrypoint": null,
            "OnBuild": null,
            "Labels": null
        },
        "Architecture": "amd64",
        "Os": "linux",
        "Size": 3655264,
        "GraphDriver": {
            "Data": null,
            "Name": "overlayfs"
        },
        "RootFS": {
            "Type": "layers",
            "Layers": [
                "sha256:3e01818d79cd3467f1d60e54224f3f6ce5170eceb54e265d96bb82344b8c24e7"
            ]
        },
        "Metadata": {
            "LastTagTime": "2025-01-01T11:39:50.804131564Z"
        }
    }
]
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
PS E:\wisdom\docker1\niginx ex> docker pull ubuntu
Using default tag: latest
latest: Pulling from library/ubuntu
de44b265507a: Download complete
Digest: sha256:80dd3c3b9c6cecb9f1667e9290b3bc61b78c2678c02cbdae5f0fea92cc6734ab
Status: Downloaded newer image for ubuntu:latest
docker.io/library/ubuntu:latest
PS E:\wisdom\docker1\niginx ex> docker run -it ubuntu
root@5a26451d235c:/# apt-get update
apt-get install -y curl
Get:1 http://archive.ubuntu.com/ubuntu noble InRelease [256 kB]
Get:2 http://security.ubuntu.com/ubuntu noble-security InRelease [126 kB]
Get:3 http://security.ubuntu.com/ubuntu noble-security/main amd64 Packages [719 kB]
Get:4 http://archive.ubuntu.com/ubuntu noble-updates InRelease [126 kB]
Get:5 http://archive.ubuntu.com/ubuntu noble-backports InRelease [126 kB]
Get:6 http://archive.ubuntu.com/ubuntu noble/main amd64 Packages [1808 kB]
Get:7 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Packages [1028 kB]
Get:8 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 Packages [707 kB]
Get:9 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 Packages [15.3 kB]
Get:10 http://archive.ubuntu.com/ubuntu noble/multiverse amd64 Packages [331 kB]
Get:11 http://archive.ubuntu.com/ubuntu noble/universe amd64 Packages [19.3 MB]
Get:12 http://archive.ubuntu.com/ubuntu noble/restricted amd64 Packages [117 kB]
Get:13 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 Packages [968 kB]
Get:14 http://archive.ubuntu.com/ubuntu noble-updates/restricted amd64 Packages [724 kB]
Get:15 http://archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 Packages [19.7 kB]
Get:16 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 Packages [1254 kB]
Get:17 http://archive.ubuntu.com/ubuntu noble-backports/universe amd64 Packages [11.9 kB]
Fetched 27.7 MB in 15s (1785 kB/s)
Reading package lists... Done
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  ca-certificates krb5-locales libbrotli1 libcurl4t64 libgssapi-krb5-2 libk5crypto3 libkeyutils1 libkrb5-3 libkrb5support0 libldap-common libldap2
  libnghttp2-14 libpsl5t64 librtmp1 libsasl2-2 libsasl2-modules libsasl2-modules-db libssh-4 openssl publicsuffix
Suggested packages:
  krb5-doc krb5-user libsasl2-modules-gssapi-mit | libsasl2-modules-gssapi-heimdal libsasl2-modules-ldap libsasl2-modules-otp libsasl2-modules-sql
The following NEW packages will be installed:
  ca-certificates curl krb5-locales libbrotli1 libcurl4t64 libgssapi-krb5-2 libk5crypto3 libkeyutils1 libkrb5-3 libkrb5support0 libldap-common libldap2
  libnghttp2-14 libpsl5t64 librtmp1 libsasl2-2 libsasl2-modules libsasl2-modules-db libssh-4 openssl publicsuffix
0 upgraded, 21 newly installed, 0 to remove and 0 not upgraded.
Need to get 3564 kB of archives.
After this operation, 9199 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 openssl amd64 3.0.13-0ubuntu3.4 [1003 kB]
Get:2 http://archive.ubuntu.com/ubuntu noble/main amd64 ca-certificates all 20240203 [159 kB]
Get:3 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 krb5-locales all 1.20.1-6ubuntu2.2 [14.0 kB]
Get:4 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libkrb5support0 amd64 1.20.1-6ubuntu2.2 [33.7 kB]
Get:5 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libk5crypto3 amd64 1.20.1-6ubuntu2.2 [81.8 kB]
Get:6 http://archive.ubuntu.com/ubuntu noble/main amd64 libkeyutils1 amd64 1.6.3-3build1 [9490 B]
Get:7 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libkrb5-3 amd64 1.20.1-6ubuntu2.2 [347 kB]
Get:8 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libgssapi-krb5-2 amd64 1.20.1-6ubuntu2.2 [143 kB]
Get:9 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libnghttp2-14 amd64 1.59.0-1ubuntu0.1 [74.3 kB]
Get:10 http://archive.ubuntu.com/ubuntu noble/main amd64 libpsl5t64 amd64 0.21.2-1.1build1 [57.1 kB]
Get:11 http://archive.ubuntu.com/ubuntu noble/main amd64 publicsuffix all 20231001.0357-0.1 [129 kB]
Get:12 http://archive.ubuntu.com/ubuntu noble/main amd64 libbrotli1 amd64 1.1.0-2build2 [331 kB]
Get:13 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libsasl2-modules-db amd64 2.1.28+dfsg1-5ubuntu3.1 [20.4 kB]
Get:14 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libsasl2-2 amd64 2.1.28+dfsg1-5ubuntu3.1 [53.2 kB]
Get:15 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libldap2 amd64 2.6.7+dfsg-1~exp1ubuntu8.1 [195 kB]
Get:16 http://archive.ubuntu.com/ubuntu noble/main amd64 librtmp1 amd64 2.4+20151223.gitfa8646d.1-2build7 [56.3 kB]
Get:17 http://archive.ubuntu.com/ubuntu noble/main amd64 libssh-4 amd64 0.10.6-2build2 [188 kB]
Get:18 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libcurl4t64 amd64 8.5.0-2ubuntu10.6 [341 kB]
Get:19 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 curl amd64 8.5.0-2ubuntu10.6 [226 kB]
Get:20 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libldap-common all 2.6.7+dfsg-1~exp1ubuntu8.1 [31.5 kB]
Get:21 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 libsasl2-modules amd64 2.1.28+dfsg1-5ubuntu3.1 [69.9 kB]
Fetched 3564 kB in 3s (1134 kB/s)
debconf: delaying package configuration, since apt-utils is not installed
Selecting previously unselected package openssl.
(Reading database ... 4379 files and directories currently installed.)
Preparing to unpack .../00-openssl_3.0.13-0ubuntu3.4_amd64.deb ...
Unpacking openssl (3.0.13-0ubuntu3.4) ...
Selecting previously unselected package ca-certificates.
Preparing to unpack .../01-ca-certificates_20240203_all.deb ...
Unpacking ca-certificates (20240203) ...
Selecting previously unselected package krb5-locales.
Preparing to unpack .../02-krb5-locales_1.20.1-6ubuntu2.2_all.deb ...
Unpacking krb5-locales (1.20.1-6ubuntu2.2) ...
Selecting previously unselected package libkrb5support0:amd64.
Preparing to unpack .../03-libkrb5support0_1.20.1-6ubuntu2.2_amd64.deb ...
Unpacking libkrb5support0:amd64 (1.20.1-6ubuntu2.2) ...
Selecting previously unselected package libk5crypto3:amd64.
Preparing to unpack .../04-libk5crypto3_1.20.1-6ubuntu2.2_amd64.deb ...
Unpacking libk5crypto3:amd64 (1.20.1-6ubuntu2.2) ...
Selecting previously unselected package libkeyutils1:amd64.
Preparing to unpack .../05-libkeyutils1_1.6.3-3build1_amd64.deb ...
Unpacking libkeyutils1:amd64 (1.6.3-3build1) ...
Selecting previously unselected package libkrb5-3:amd64.
Preparing to unpack .../06-libkrb5-3_1.20.1-6ubuntu2.2_amd64.deb ...
Unpacking libkrb5-3:amd64 (1.20.1-6ubuntu2.2) ...
Selecting previously unselected package libgssapi-krb5-2:amd64.
Preparing to unpack .../07-libgssapi-krb5-2_1.20.1-6ubuntu2.2_amd64.deb ...
Unpacking libgssapi-krb5-2:amd64 (1.20.1-6ubuntu2.2) ...
Selecting previously unselected package libnghttp2-14:amd64.
Preparing to unpack .../08-libnghttp2-14_1.59.0-1ubuntu0.1_amd64.deb ...
Unpacking libnghttp2-14:amd64 (1.59.0-1ubuntu0.1) ...
Selecting previously unselected package libpsl5t64:amd64.
Preparing to unpack .../09-libpsl5t64_0.21.2-1.1build1_amd64.deb ...
Unpacking libpsl5t64:amd64 (0.21.2-1.1build1) ...
Selecting previously unselected package publicsuffix.
Preparing to unpack .../10-publicsuffix_20231001.0357-0.1_all.deb ...
Unpacking publicsuffix (20231001.0357-0.1) ...
Selecting previously unselected package libbrotli1:amd64.
Preparing to unpack .../11-libbrotli1_1.1.0-2build2_amd64.deb ...
Unpacking libbrotli1:amd64 (1.1.0-2build2) ...
Selecting previously unselected package libsasl2-modules-db:amd64.
Preparing to unpack .../12-libsasl2-modules-db_2.1.28+dfsg1-5ubuntu3.1_amd64.deb ...
Unpacking libsasl2-modules-db:amd64 (2.1.28+dfsg1-5ubuntu3.1) ...
Selecting previously unselected package libsasl2-2:amd64.
Preparing to unpack .../13-libsasl2-2_2.1.28+dfsg1-5ubuntu3.1_amd64.deb ...
Unpacking libsasl2-2:amd64 (2.1.28+dfsg1-5ubuntu3.1) ...
Selecting previously unselected package libldap2:amd64.
Preparing to unpack .../14-libldap2_2.6.7+dfsg-1~exp1ubuntu8.1_amd64.deb ...
Unpacking libldap2:amd64 (2.6.7+dfsg-1~exp1ubuntu8.1) ...
Selecting previously unselected package librtmp1:amd64.
Preparing to unpack .../15-librtmp1_2.4+20151223.gitfa8646d.1-2build7_amd64.deb ...
Unpacking librtmp1:amd64 (2.4+20151223.gitfa8646d.1-2build7) ...
Selecting previously unselected package libssh-4:amd64.
Preparing to unpack .../16-libssh-4_0.10.6-2build2_amd64.deb ...
Unpacking libssh-4:amd64 (0.10.6-2build2) ...
Selecting previously unselected package libcurl4t64:amd64.
Preparing to unpack .../17-libcurl4t64_8.5.0-2ubuntu10.6_amd64.deb ...
Unpacking libcurl4t64:amd64 (8.5.0-2ubuntu10.6) ...
Selecting previously unselected package curl.
Preparing to unpack .../18-curl_8.5.0-2ubuntu10.6_amd64.deb ...
Unpacking curl (8.5.0-2ubuntu10.6) ...
Selecting previously unselected package libldap-common.
Preparing to unpack .../19-libldap-common_2.6.7+dfsg-1~exp1ubuntu8.1_all.deb ...
Unpacking libldap-common (2.6.7+dfsg-1~exp1ubuntu8.1) ...
Selecting previously unselected package libsasl2-modules:amd64.
Preparing to unpack .../20-libsasl2-modules_2.1.28+dfsg1-5ubuntu3.1_amd64.deb ...
Unpacking libsasl2-modules:amd64 (2.1.28+dfsg1-5ubuntu3.1) ...
Setting up libkeyutils1:amd64 (1.6.3-3build1) ...
Setting up libbrotli1:amd64 (1.1.0-2build2) ...
Setting up libsasl2-modules:amd64 (2.1.28+dfsg1-5ubuntu3.1) ...
Setting up libpsl5t64:amd64 (0.21.2-1.1build1) ...
Setting up libnghttp2-14:amd64 (1.59.0-1ubuntu0.1) ...
Setting up krb5-locales (1.20.1-6ubuntu2.2) ...
Setting up libldap-common (2.6.7+dfsg-1~exp1ubuntu8.1) ...
Setting up libkrb5support0:amd64 (1.20.1-6ubuntu2.2) ...
Setting up libsasl2-modules-db:amd64 (2.1.28+dfsg1-5ubuntu3.1) ...
Setting up librtmp1:amd64 (2.4+20151223.gitfa8646d.1-2build7) ...
Setting up libk5crypto3:amd64 (1.20.1-6ubuntu2.2) ...
Setting up libsasl2-2:amd64 (2.1.28+dfsg1-5ubuntu3.1) ...
Setting up libkrb5-3:amd64 (1.20.1-6ubuntu2.2) ...
Setting up openssl (3.0.13-0ubuntu3.4) ...
Setting up publicsuffix (20231001.0357-0.1) ...
Setting up libldap2:amd64 (2.6.7+dfsg-1~exp1ubuntu8.1) ...
Setting up ca-certificates (20240203) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
debconf: unable to initialize frontend: Readline
debconf: (Can't locate Term/ReadLine.pm in @INC (you may need to install the Term::ReadLine module) (@INC entries checked: /etc/perl /usr/local/lib/x86_64-linux-gnu/perl/5.38.2 /usr/local/share/perl/5.38.2 /usr/lib/x86_64-linux-gnu/perl5/5.38 /usr/share/perl5 /usr/lib/x86_64-linux-gnu/perl-base /usr/lib/x86_64-linux-gnu/perl/5.38 /usr/share/perl/5.38 /usr/local/lib/site_perl) at /usr/share/perl5/Debconf/FrontEnd/Readline.pm line 8.)
debconf: falling back to frontend: Teletype
Updating certificates in /etc/ssl/certs...
146 added, 0 removed; done.
Setting up libgssapi-krb5-2:amd64 (1.20.1-6ubuntu2.2) ...
Setting up libssh-4:amd64 (0.10.6-2build2) ...
Setting up libcurl4t64:amd64 (8.5.0-2ubuntu10.6) ...
Setting up curl (8.5.0-2ubuntu10.6) ...
Processing triggers for libc-bin (2.39-0ubuntu8.3) ...
Processing triggers for ca-certificates (20240203) ...
Updating certificates in /etc/ssl/certs...
0 added, 0 removed; done.
Running hooks in /etc/ca-certificates/update.d...
done.
root@5a26451d235c:/# curl --version
curl 8.5.0 (x86_64-pc-linux-gnu) libcurl/8.5.0 OpenSSL/3.0.13 zlib/1.3 brotli/1.1.0 zstd/1.5.5 libidn2/2.3.7 libpsl/0.21.2 (+libidn2/2.3.7) libssh/0.10.6/openssl/zlib nghttp2/1.59.0 librtmp/2.3 OpenLDAP/2.6.7
Release-Date: 2023-12-06, security patched: 8.5.0-2ubuntu10.6
Protocols: dict file ftp ftps gopher gophers http https imap imaps ldap ldaps mqtt pop3 pop3s rtmp rtsp scp sftp smb smbs smtp smtps telnet tftp
Features: alt-svc AsynchDNS brotli GSS-API HSTS HTTP2 HTTPS-proxy IDN IPv6 Kerberos Largefile libz NTLM PSL SPNEGO SSL threadsafe TLS-SRP UnixSockets zstd
root@5a26451d235c:/# exit
exit
