# buzzmachines

## intro
Buzzmachines are audio generators and effects using an API designed by the free
modular software music studio "Jeskola Buzz". (see http://jeskola.net/buzz/ and
http://www.buzzmachines.com).

This module provides a set of buzzmachines that have been published in source
code form on the internet. The aims of the project are:
* allow to rebuild the machines for new platforms (e.g. 64bit, new compiler
  versions, etc.)
* fix bugs (crashers, dc offsets, denormals)
* improve performance (smarter algorithms)
* be a good resource for developers that want to write new machines

## building on windows
FIXME

## building on linux
To build use autogen.sh instead of configure. This accept the same options like
configure. Later one can use autoregen.sh to rerun the bootstrapping.

They can be used via bml library or in all gstreamer app via bml+gst-buzztrax
(see http://www.buzztrax.org)
You can install this module locally too. Use following option for
./autogen.sh or ./configure

    --prefix=$HOME/buzztard/

Add the path to the BML_PATH env var:

    export BML_PATH=$HOME/buzztard/lib/Gear:$HOME/buzztard/lib/Gear/Effects:\
      $HOME/buzztard/lib/Gear/Generators

The native machines will be installed to $prefix/lib/Gear.
