First you need to create a ```.list``` file in your ```sources.list.d``` directory. To do that execute the following command.
```
sudo tee /etc/apt/sources.list.d/pritunl.list
```
After writing this command just press enter and then you will go to next line, Here you have to write the content of the file ```pritunl.list``` which you have created.
Now just write the below command
```
deb https://repo.pritunl.com/stable/apt focal main
```
Now press the ```ENTER``` button and it will show you the same ommand which you have typed.

Now you need to enter your key
```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv WRITE--YOUR--KEY--HERE
```

After you will enter your key and press enter it will show below output
```
Executing: /tmp/apt-key-gpghome.3cosYfk24l/gpg.1.sh --keyserver hkp://keyserver.ubuntu.com --recv YOUR-KEY
gpg: key YOUR-KEY: public key "Pritunl <contact@pritunl.com>" imported
gpg: Total number processed: 1
gpg:               imported: 1

```

Now execute the following command
```
sudo apt-get update
sudo apt-get install pritunl-client-electron
```
Use the following key: ```7568D9BB55FF9E5287D586017AE645C0CF8E292A```
This key has been taken from official pritunl site.
