LOCAL_MANIFEST
========================
Project for motorola Moto G 2015  (OSPREY)

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
    $ repo init -u https://github.com/temasek/android.git -b cm-13.0
    $ curl --create-dirs -L -o .repo/local_manifests/aospa.xml -O -L https://raw.githubusercontent.com/RolanDroid/local_manifest/aospa/aospa.xml
```
### For sync: ###
```bash
    $ repo sync -j4
```
### To build for your device.. ###
```bash
    $ build/envsetup.sh
    $ brunch device_name_here
```


