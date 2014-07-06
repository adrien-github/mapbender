Mapbender bends a map along a path.


# Requirements

On Debian systems you need the following packages:

	apt-get install python python-pil python-scipy python-tk python-matplotlib python-numpy
	
In order to download the tiles with the -d option, you also need landez (not packaged on Debian):

    apt-get install python-setuptools
    easy_install landez
 
https://github.com/makinacorpus/landez

# Usage

All the configuration is made in config.ini (a sample file is provided)

I use this workflow to generate the map:

- Create a GPX track, for instance with openrunner.com
- modify the config.ini (filename, parameters)
- launch the program. You need to use -d option the first time, to download the tiles.

  ./mapbender -d
  
Be carefull, it will download the tiles in /tmp/landez, and can be quite big.

- transform the image produced in PDF with PosteRazor

Now you may have a good map to travel :)

# Know how it works

The first author explain it on his blog:

https://blog.mister-muffin.de/2014/04/03/mapbender---maps-for-long-distance-travels/
