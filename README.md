# Sudoku for SailfishOS

This is a Sudoku application for SailfishOS.

# Reporting Issues

If you're having an issue with the Sudoku application, please do one of the following:

## Report it here on GitHub

If you have an account on GitHub, or you don't mind creating one, you can file the issue here directly.

## E-mail me

You can contact me at the address available on my website: http://hoelz.ro

Please don't leave bug reports in the store comments; I don't get notifications for them, and I only
check them every few months!

# Building & Installing

You can build the application from QtCreator distributed with the Sailfish SDK, or you can build it
from the command line:

## Start the MerSDK Virtual Machine

    user@machine $ VBoxManage startvm MerSDK

## SSH into the MerSDK VM

    user@machine $ ssh -i ~/SailfishOS/vmshare/ssh/private_keys/engine/mersdk mersdk@localhost -p 2222

## Run the build process to generate an RPM

    mersdk@mersdk $ mb2 -t SailfishOS-armv7hl build

## Copy the RPM to your phone

    user@machine $ scp RPMS/harbour-sudoku*.rpm jolla:

## Install on your phone

    root@jolla $ rpm -Uvh harbour-sudoku*.rpm
