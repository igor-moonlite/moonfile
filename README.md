# MoonFile

[AfterLogic WebMail Lite](https://afterlogic.org/webmail-lite) is a free webmail application.

[MoonLite](https://github.com/igor-moonlite/moonlite/) is a fat-free fork of AfterLogic WebMail Lite.

MoonFile is extended edition of MoonLite, with Files added.

## Installing MoonFile from APT repository

1. Add this to your `/etc/apt/sources.list` file:
```
deb http://apt.mooncats.ru /
```

2. Install a public key:
```
curl -s http://apt.mooncats.ru/moonlite.asc | sudo gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/moonlite.gpg --import
chmod 644 /etc/apt/trusted.gpg.d/moonlite.gpg
```

3. Update APT cache:
```
apt update
```

4. Install MoonFile:
```
apt install moonfile
```

The package and repository are built with [this tool here](https://github.com/igor-moonlite/apt-build).

## Installing MoonFile from ZIP package

1. Download the package at https://mooncats.ru/download/moonfile.zip

2. For fresh installation, extract the package to web directory. Make sure webserver is able to write in data subdirectory.

3. For upgrade, backup `data` subdirectory; if you made any changes to `content` you may wish to backup as well. Delete the installation, extract the package and restore from backup.

4. In web browser, navigate to `/adminpanel/`, default login is superadmin, with an empty password.
