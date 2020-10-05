---
title: "HPC Setup"
sidebar: toc
maxdepth: 1
sort: 5
---


# High Performance Computing Cluster

---

A high performance computing cluster allows multiple users to invest in a multi-core computing envirnment. It should also reduce tedium of installing commonly used software (in theory).

Logging into a HPC, usually requires some kind of secure shell call (`ssh`) whether it's through a GUI (putty) or a terminal (command line). The general format is usually

```
ssh username@serverlocation.com
```

Where it will ask for your password and maybe an authentication key.

For some reason, the home directory for users tends to have limited space (~5GB) so to make like easier, it's best to link folders to your home folder.

```
ln -s /project/yourprojectname .
cd /project/yourprojectname
mkdir .conda      # For miniconda environments
mkdir .Rlibraries # For R libraries
cd
ln -s /project/yourprojectname/.conda .
ln -s /project/yourprojectname/.Rlibraries .
```
