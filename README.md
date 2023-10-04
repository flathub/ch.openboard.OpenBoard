# Flatpak packaging for OpenBoard

This repository contains the flatpak packaging files for [OpenBoard](https://openboard.ch).

## Maintainance

OpenBoard only officially targets Ubuntu LTS with its own packaging scripts.
The buildsystem is therefore missing a number of things needed for
the more standard install locations inside flatpak and the more recent dependencies used here.

Due to the rather high number of patches, they are maintained in a [separate git repository](https://gitlab.com/JBBgameich/OpenBoard/-/commits/master).
The `master` branch always contains the latest packaged tag, plus the required patches.
They can be exported for use in the packaging using `git format-patch v1.6.4` (or a newer tag).
The branch should be rebased on top of the latest tag when needed, and can then be force-pushed.
