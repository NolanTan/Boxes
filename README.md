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
- boxes input.txt -s 80x15 -a jc
- boxes input.txt -s 80x15 -a jr
- boxes input.txt -s 80x15 -a jrvb
- boxes input.txt -s 80x15 -a jrvt
- boxes input.txt -s 80x15 -a jcvbhr

#### alignment shortcuts
- boxes input.txt -s 80x15 -a l
- boxes input.txt -s 80x15 -a r
- boxes input.txt -s 80x15 -a c

#### padding
- boxes input.txt -p h8v9
- boxes input.txt -p h8v9 -a vb (doesn't work because padding applies to inside box)
- boxes input.txt -p a5r0

#### prebuilt boxes
- boxes -l (list)
- boxes -q color (query)
- echo "Don't do that" | boxes -d critical
- boxes -d whirly input.txt
- echo "This is my message" | boxes -d xes

#### custom box configuration files
- echo "Hello Everyone" | boxes -f my-boxes-config
- vim my-boxes-config
- echo "Hello Everyone" | boxes -f my-boxes-config -d oh

#### mend
- echo "Hi" | boxes -d cowsay
- vim broken.txt
- boxes -d cowsay -m broken.txt

#### remove
- cat cow.txt
- cat cow.txt | boxes -r (auto detection fails)
- cat cow.txt | boxes -r -d cowsay

#### create (shortcut for regional comments)
- boxes -c // input.txt

#### vim configuration
- cat ~/.vimrc
- vim HelloWorld.java
- ,mc


