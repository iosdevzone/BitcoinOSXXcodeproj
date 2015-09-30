# BitcoinOSXXcodeproj
An Xcode project for compiling and debugging Bitcoin Core.

# How to use it

Clone bitcoin and this repository into the same directory.
Run the install.sh script to copy the Xcode project into <bitcoin_root>/contrib/osx.

```shell
mkdir BitcoinExperiments
cd BitcoinExperiments
git clone https://github.com/bitcoin/bitcoin.git
git clone https://github.com/iosdevzone/BitcoinOSXXcodeproj.git
pushd BitcoinOSXXcodeproj
./install.sh
popd
open bitcoin/contrib/osx/BitcoinOSX.xcodeproj
```

# Caveats

This projects assumes that all external dependencies (e.g. Berkeley DB, boost and libevent) are in their default locations as installed by homebrew. If this is not the case, you will need to modify the project to point to the correct locations. This is an incredibly tedious process.
