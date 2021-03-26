*Snap package of Folding@Home*

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-white.svg)](https://snapcraft.io/folding-at-home-fcole90)

**Builds:** [![.github/workflows/package_and_release.yml](https://github.com/fcole90/fah-snap/actions/workflows/package_and_release.yml/badge.svg)](https://github.com/fcole90/fah-snap/actions/workflows/package_and_release.yml)

<a href="https://snapcraft.io/folding-at-home-fcole90" target="_blank">
  <img src="https://user-images.githubusercontent.com/1292230/83427711-d319dc80-a439-11ea-949f-95fafa805886.png" />
</a>

## How can I install Folding at Home?
```
sudo snap install folding-at-home-fcole90 # Install
snap connect folding-at-home-fcole90:hardware-observe # Allow checking your hardware (Should now be autoconnected)
```
The `hardware-observe` connection allows the Folding at home to access information on your hardware, which it requires to
detect your GPUs correctly.

<!--
## How can I use Folding at Home as a daemon?
You can interact with the daemon service with:
```
snap services folding-at-home-fcole90.client # Check that the service is running correctly
```
**Note**: the daemon is disabled by default, because otherwise it would start upon install, without any notification.
I think this is not what most users expect. You can start it and enable autostart with the following:
```
snap start --enable folding-at-home-fcole90.client # Starts the service and enables autostart
```
See how to handle snap services: https://snapcraft.io/docs/service-management
The daemon is started by systemd, and is owned by root. The data folder for this is defined by `$SNAP_COMMON`,
which usually expands to `/var/snap/folding-at-home-fcole90/common`
See more on this on https://snapcraft.io/docs/environment-variables
-->

<!--
## How can I use Folding at Home as a userspace service?
If you are not using the daemon, you can either activate it or you can use the userspace service. You can run the userspace service launching `folding-at-home-fcole90` in your terminal. The data folder for this defined by `$SNAP_USER_COMMON`,
which usually expands to `home/$USERNAME/snap/folding-at-home-fcole90/common`.
See more on this on https://snapcraft.io/docs/environment-variables
This is currently unintuitive, I'm working in my spare time on improving the user experience.
-->

## How can I interact with the service using the GUI?
You can just launch `FAHControl` from your applications or from terminal:
```
folding-at-home-fcole90.FAHControl
```

If it says that no client is running, you can activate the client from a terminal:
```
folding-at-home-fcole90
```

# Folding@Home - Help research with distributed computing.

**I am One in a Million**: Regardless if you are already folding or haven’t heard a word about 
it before, we need your help to reach our goal – which is 1 million folders.
**Start folding now**

## What is it?
**Folding@home (FAH or F@h)** is a distributed computing project for simulating protein dynamics, 
including the process of protein folding and the movements of proteins implicated in a variety of diseases.
It brings together citizen scientists who volunteer to run simulations of protein dynamics on their personal computers. 
Insights from this data are helping scientists to better understand biology, and providing new opportunities 
for developing therapeutics.

## More info
Folding@Home is run by Pandegroup of Stanford University. You can find more information on 
the Folding@Home [website](https://foldingathome.org/about/).

## Metrics as of March 2021
<a href="https://snapcraft.io/folding-at-home-fcole90" target="_blank">
  <img src="https://user-images.githubusercontent.com/1292230/112675832-53e61100-8e70-11eb-8d05-f5b687bf25b3.png" />
  <img src="https://user-images.githubusercontent.com/1292230/112675686-24370900-8e70-11eb-85e5-5cd5afdea827.png" />
</a>

