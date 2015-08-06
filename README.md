# Kartesio
Program for calculating best fit curves for a set of experimental points using regression algorithms and neural networks.

This repository contains the source code of Kartesio and ZorbaNeuralNetwork.
If you are looking for ready to use binary packages, please take a look at https://github.com/zorbaproject/kartesio-build

<h4>
DEBIAN PACKAGING:
</h4>
To create a Debian package of Kartesio, just enter the source code directory (named for example "kartesio-1.0") and run the following commands:
<br><i>
dh_make -e TRINGALINVENT@libero.it -s --createorig
<br>
debuild -S -sa
<br>
debuild binary
</i> <br>
You'll find the binary package for your architecture in the up level directory ("cd ../").

Of course, you'll need to edit the files "debian/control" and "debian/changelog" with your email address and your name, so you can sign the packages with your PGP key.
If you made some changes to Kartesio source code, and you need to find out which libraries are needed to let the program work, you can just run the following command:
<br><i>
./list-libraries.sh
</i> <br>
To use this command, you'll need to install the program apt-file (with "sudo apt-get install apt-file").
