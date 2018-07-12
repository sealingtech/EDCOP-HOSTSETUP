# Host Setup

This github repository is a supporting component of EDCOP.  This contains a container designed to be used as a daemonset to configure hosts.  The image is based on Centos and is used in configure-sensors (https://github.com/sealingtech/EDCOP-CONFIGURESENSORS) but can be used for other purposes. 

Pass in an environment variable which contains an executable shell script. This script will then run to completion and continue to run doing nothing.  The purpose of this is to ensure that the script runs again when hosts reboot.  For an example of how to do this: https://github.com/sealingtech/EDCOP-CONFIGURESENSORS/blob/master/configure-sensors/templates/configure-sensors-daemsonset.yaml