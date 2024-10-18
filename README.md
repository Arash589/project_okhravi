# Arduino IDE project 

If you like Arduino, but also like to use your text editor of choice and you're not afraid of the command line, this project is for you! Like many others I started programming micro-controllers using the Arduino IDE. But after a while I started to dislike the default editor. For a while I used an Arduino Makefile to compile my code. Until recently I found out that the current version (as of May 2016) of the Arduino IDE also has a command line interface. (See [documentation](https://github.com/arduino/Arduino/blob/master/build/shared/manpage.adoc))

# Dependencies

* Arduino IDE >= 1.5
* bash or zsh
* minicom     (optional)
* git         (optional)

# Structure

The structure of your new Arduino project is as follows:

```shell
.
├── doc                 Aditional documentation file
├── libraries           Arduino library files
├── main                Main sketch file
│   └── main.ino        Main Arduino sketch
├── LICENCE.txt         Licence file
├── config.sh           Arduino config file
└── README.md           Project README file
```

You (main) sketch goes in `main/main.ino`. This is where `void setup()` and `void loop()` live. Your libraries (dependencies) go into the libraries folder. You can ether copy your libraries here or symlink them. If you have additional documentation, like datasheets for example, they go into the `doc` folder.
