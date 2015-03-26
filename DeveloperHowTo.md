# Introduction #

This is a brief explanation of how to use the code after checking out from svn.


# Checkouts #

Normally you want to check out from trunk/ unless you are working on a specific branch or want to build a certain release tag. The project actually contains two Gambas projects, as Gambas does not support multi-application development within a single project. So when you checkout, you get 2 directories, which correspond to those 2 Gambas projects, vcpufreq-gui and vcpufreq-loader.


# Hacking #

To work on the code you need Gambas 1.0.x, development is now done in 1.0.17, so that is the recommended version. One of the goals of the project is to keep the number of Gambas GUI components needed to a minimum, preferably just the QT component, to facilitate porting to GTK once Gambas2 goes stable.


# Packaging #

The binaries resulting from compilation of both projects should be packaged together, vcpufreq (from vcpufreq-gui) should go in /usr/bin and vcpufreq-load (from vcpufreq-loader) should go in /usr/sbin (except in Vector Linux, where it is placed in /sbin as it is considered "native" to this distro).