# HDR Image Recognition

## Setup
When you [install Python](https://www.python.org/getit/), be sure to check "Add Python 3.x to PATH" so that you can run Python from the terminal. This will also install `pip`, the package management tool for Python that makes it easy to install libraries.

In Windows, open the Powershell (a more robust terminal) by right-clicking the Powershell icon in the taskbar (Looks like this: ![Powershell icon](icons/powershell.jpg)) and selecting "Run as Administrator." Then navigate to this repo, which probably looks something like this in Windows:

	cd c:\Users\[your name]\Desktop\HDR-images

To get the libraries we need, just run:

	pip3 install -r requirements.txt

This will install [Jupyter](http://jupyter.org/), a sophisticated Python interface that makes coding much easier. Once that's done, you can start the notebook with this command:

	jupyter notebook

This will open a browser window with all the notebooks in this directory.

## Scripts

`inspectTIFF.ipynb` simply checks the metadata from a sample TIF to see if there's anything we're missing. Based on the output, it looks like a standard 1008x1018 pixel image:

	Key: Image SubfileType, value Full-resolution Image
	Key: Image ImageWidth, value 1008
	Key: Image ImageLength, value 1018
	Key: Image BitsPerSample, value 16
	Key: Image Compression, value Uncompressed
	Key: Image RowsPerStrip, value 4
	Key: Image XResolution, value 72
	Key: Image YResolution, value 72