# BOXES Linux Tool Demo

Nolan Flinchum and Yazmin Cosme Escobedo
Western Carolina University
4/17/2024

## Description

Preparing for a demo of the Linux tool 'boxes'.

## Tests to Remember

#### basics
- boxes input.txt
- echo "This is my message" | boxes
- boxes -> Hello -> Ctrl D (not typical)

#### prebuilt boxes
- boxes -l (list)
- boxes -q color (query)
- echo "Don't do that" | boxes -d critical
- boxes -d whirly input.txt
- echo "This is my message" | boxes -d xes

#### alignment
- echo "This is my message" | boxes -d xes -a vb
- echo "This is my message" | boxes -d xes -a vc
- echo "This is my message" | boxes -d xes -a vcjr (jr won't work)
- echo "This is my message: | boxes -d xes -a vchr (will work)
- boxes -d xes -a vchrjr input.txt (properly show jr)

#### alignment shortcuts
- boxes -d xes -a r input.txt
- boxes -d xes -a c input.txt
- boxes -d xes -a l input.txt

#### padding
- boxes input.txt -p h8v9
- boxes input.txt -p a5r0

#### custom box configuration files
- echo "Hello Everyone" | boxes -f my-boxes-config
- vim my-boxes-config
- echo "Hello Everyone" | boxes -f my-boxes-config -d oh

#### mend
- echo "Hi" | boxes -d cowsay
- vim broken.txt
- boxes -d cowsay -m broken.txt
