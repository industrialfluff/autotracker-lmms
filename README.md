# autotracker-lmms
Procedural generation of songs for LMMS based on the previous autotracker-bottomsup code.

# Requirements
Python 3.10+, the old code is stuck at Python 2.7 and this is the time to upgrade.

# Overview
The old code creates a binary bitpacked format for Impulse Tracker.  LMMS uses XML files, so it is much easier to create the files.

Also, Impulse Tracker allow multiple samples per track, while each track in LMMS seems to be one sample.  So it's better to start out with fresh code.

Impulse Tracker modules also embedded the samples in the file, LMMS does not.  This means all the samples, soundfonts, etc. need file references outside the module. This can get tricky when moving modules between PCs.
