# RRRJ Overlay

## Install Overlay

```
root # layman \
-o https://raw.githubusercontent.com/robertov82008/rrrj/master/profiles/repositories.xml \
-f \
-a rrrj-overlay
```

`root # layman-updater -R`


### update

`root # emerge --sync`

`root # layman -S`

`root # eix-sync -q`


## Create your overlay

`$ git clone project-overlay`

#### Sets your changes

`project-overlay $ git add . && git commit -m 'init`

`project-overlay- $ git push`

`root # layman-overlay-maker`

#### Generate Manifest

`project/category/app $ ebuild app.ebuild manifest`
