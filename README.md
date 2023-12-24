# Upgrade-Autonity-v0.12.3-prerelease 

#To update Autonity to version 0.12.3-pre, you can follow the steps below:

Clone the Autonity source code from GitHub:

    git clone https://github.com/autonity/autonity.git

Navigate to the Autonity directory:

    cd autonity

Switch to version 0.12.3-pre:

    git checkout tags/v0.12.3-pre -b v0.12.3-pre

Install and build Autonity:

    make autonity

Stop the current Autonity service:

    systemctl stop autonityd

Copy the executable file to the /usr/local/bin/ directory and grant execution permission:

    cp -rf build/bin/autonity /usr/local/bin/autonity && chmod +x /usr/local/bin/autonity

Update the system daemon:

    systemctl daemon-reload

Restart the Autonity service:

    systemctl restart autonityd


Note: Make sure you have the necessary permissions to make these changes, and ensure that you have backed up important data before performing any updates.
