This is [**GenX**](http://genx.sourceforge.net/), which is a X-ray and Neutron reflectivity fitting program and originally written by **Matts Björck**, ported to Python 3 and wxPython Phoenix by me. Codes that were originally dependent on scipy.weave were re-written in Cython. Some caveats of this version include the following:
1. I have only tested on GNU/Linux, however there is no reason why it will not work on other platforms. The code itself should be platform-neutral, and only `setup.py` needs to be modified in order to install the program on other platforms.
2. While this Python 3 version can open both the .gx and .hgx files saved by the Python 2 version, it can not save the .gx files due to the change in the Python pickle protocol. I have changed the extension of the saved files from .gx to .gx3 to highlight this incompatibility. If interoperability with the Python 2 version is desired, please use .hgx format.  

Apart from the save file caveat mentioned above, this version is compatible with **both** Python 2 and Python 3, provided wxPython Phoenix is installed. To install this program, please run either `sudo python2 setup.py install` or `sudo python3 setup.py install`, depending on the Python version. A PKGBUILD for Arch Linux can be found from the AUR.
