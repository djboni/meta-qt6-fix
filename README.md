# Fixes for meta-qt6

GitHub: https://github.com/djboni/meta-qt6-fix

Yocto meta layer with fixes for the layer meta-qt6.

I had some issues building the Qt6 toolchain in with Yocto.
Here is the layer I made to fix the issues.

Example:

Clone the meta layers (I was using the branch 6.7 on meta-qt6):

```console
$ git clone https://code.qt.io/yocto/meta-qt6 -b 6.7
$ git clone https://github.com/djboni/meta-qt6-fix
```

Add both meta layers to build/conf/bblayers.conf.

TODO: Is there a command that does that?

Build:

```console
$ bitbake meta-toolchain-qt6
```

