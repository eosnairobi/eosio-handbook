# **Introduction**

_This is a step by step walk through on how to clone, build and run a single node on your machine, handling all the small issues you may face along the way._

**Step 1**. **Clone EOS**

```
git clone https://github.com/EOSIO/eos --recursive
```

Just be patient, this may take a while.

**Step 2. Checkout the appropriate Tag**

If you follow the tutorial on [developers.eos.io](https://developers.eos.io "EOSIO Developers&apos; Guide"), you will have to checkout `v1.0.0`. In this tutorial, we start with the same tag \(`v1.0.0`, but we shall do another one soon enough\).

* [x] `git checkout v1.0.0`

* [x] You may bump into an error, with Git complaining that your `libraries/fc` folder would be overwritten. You can use the conventional way to solve this, but for me, I just deleted the damn `libraries/fc` folder with `rm -rf libraries/fc`

* [x] So now try git checkout v1.0.0. You may \[definitely\] bump into another issue, but running this will fix`git submodule update --init  --recursive`



