THEA-LOCAL_MANIFEST
========================
Project for motorola Moto G 2014 LTE (THEA)

### Installing Repo ###
```bash
# Make a directory where Repo will be stored and add it to the path
    $ mkdir ~/.bin
    $ PATH=~/.bin:$PATH

# Download Repo itself
    $ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo

# Make Repo executable
    $ chmod a+x ~/.bin/repo
```

### Initializing Repo ###
```bash
    $ repo init -u https://github.com/AICP/platform_manifest.git -b mm6.0
### For AICP normal build: ###
    $ curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.githubusercontent.com/RolanDroid/local_manifest/aicp-6.0/local_manifest.xml
```
### For sync: ###
```bash
    $repo sync -j4
```
### To build for your device.. ###
```bash
    $ . build/envsetup.sh
    $ brunch device_name_here
```


