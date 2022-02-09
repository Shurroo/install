# Shurroo install

# Motivation
We need a convenient way to bootstrap the Shurroo installation process, and resolve dependency loops, where `package1` is needed to install `package2`, but `package2` is needed to install `package1`.

# Install location
For valid security reasons, macOS is restricting user account access to locations outside the user's home folder, so we install to `~/.shurroo`. 

# Script actions

* Test the current machine status, and then if required
* Install XCode Command Line Tools (CLT)
* Create `.shurroo` in the user home folder
* Install or upgrade the principal `shurroo` repo to `.shurroo`
* Create other working folders within `.shurroo`

# Usage
```shell
/bin/bash -c "$(curl -fsSL https://https://raw.githubusercontent.com/Shurroo/install/master/install.sh)"
```

# License

BSD

# Author Information

Ian Taylor ([IanTaylorFB](https://github.com/IanTaylorFB)), Co-Founder and CTO at [FlyingBinary Ltd](https://flyingbinary.com).
