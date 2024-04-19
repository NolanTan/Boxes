# BOXES Linux Tool Demo

- Nolan Flinchum and Yazmin Cosme Escobedo
- Western Carolina University
- 4/17/2024

## Description

- Preparing for a demo of the Linux tool 'boxes'.

## Tests to Remember

#### basics
- boxes input.txt
- echo "This is my message" | boxes
- boxes -> Hello -> Ctrl D (not typical)

#### size
- boxes input.txt
- boxes input.txt -s 80x15

#### alignment
- boxes input.txt -s 80x15 -a jcvbhr
- boxes input.txt -s 80x15 -a r
- boxes input.txt -s 80x15 -a c

#### padding
- boxes input.txt -p h8v9
- boxes input.txt -p a5r0

#### prebuilt boxes
- boxes -l (list)
- boxes -q color (query)
- boxes -d xes input.txt

#### custom box configuration files
- echo "Hello Everyone" | boxes -f my-boxes-config
- vim my-boxes-config
- echo "Hello Everyone" | boxes -f my-boxes-config -d oh

#### vim configuration
- cat ~/.vimrc
- vim HelloWorld.java
- ,mc

#### mend
- echo "Hi" | boxes -d cowsay
- vim broken.txt
- boxes -d cowsay -m broken.txt

#### remove
- cat cow.txt
- cat cow.txt | boxes -r (auto detection fails)
- cat cow.txt | boxes -r -d cowsay