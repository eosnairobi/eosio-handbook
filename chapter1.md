# Basic Setup Instructions

_This is a step by step walk through on how to clone, build and run a single node on your machine, handling all the small issues you may face along the way._

**Step 1**. **Clone EOS**

```
git clone https://github.com/EOSIO/eos --recursive
```

Just be patient, this may take a while.

**Step 2. Checkout the appropriate Tag**

If you follow the tutorial on [developers.eos.io](https://developers.eos.io "EOSIO Developers&apos; Guide"), you will have to checkout `v1.2.4`. In this tutorial, we start with the same tag \(`v1.2.4`, but we shall do another one soon enough\).

* [x] `git checkout v1.2.4`

* [x] You may bump into an error, with Git complaining that your `libraries/fc` folder would be overwritten. You can use the conventional way to solve this, but for me, I just deleted the damn `libraries/fc` folder with `rm -rf libraries/fc`

* [x] So now try git checkout _**v1.2.4**_. You may \[definitely\] bump into another issue, but running this will fix`git submodule update --init  --recursive`

**Step 3. Build EOS**

If all went smoothly on step 2, you should be able to build \_**eos **\_successfully in this step.

Navigate to the folder where you have cloned eos.

```bash
shalomz@shalomz ~ $ cd /path/to/eos
```

We expect to see the following structure in the folder:

```
shalomz@shalomz ~/Projects/EOS/eos $ ls
build           eos.doxygen.in      images      testnet.template
CMakeLists.txt  eosio_build.sh      libraries   tests
CMakeModules    eosio_install.sh    LICENSE     tools
contracts       eosio_uninstall.sh  plugins     tutorials
data            eosio.version.in    programs    unittests
debian          README.md
Docker          externals           scripts
docs            HEADER              testnet.md
```

In this step, we are interested in two scripts:

```
eosio_build.sh
```

and

```
eosio_install.sh
```

The `eosio_build.sh` script does exactly what the name suggests: it is an automated build script that makes it easy for us to compile eos.

Since it is executable, \(if not, just run `sudo chmod +x eosio`\_`build.sh`\) we \_run

```bash
shalomz@shalomz ~/Projects/EOS/eos $ sudo ./eosio_build.sh
```

This will build eos and shall install any missing but required dependency.



