# Interactive Transits
This code provides a way to interactively visualize exoplanet transits with a webcam (or phone camera). Point the camera at a solid color source (default is red) and then place object in the way to see the plot respond the source being obscured. 


## Dependencies
The only packages required for these scripts to execute are:\
numpy \
matplotlib \
h5py \
opencv-python

opencv-python is the only module that may pose problems. Make sure h5py is installed in your enivoronment first, then run \
`pip install opencv-python`

For more information see: https://pypi.org/project/opencv-python/


## Video Streaming Options

### Laptop Webcam
This is the simplest to execute, using you laptop's native webcam instead of an external phone. Simply execute `transit_plot_laptop.py` to use your laptop webcam. This is a great option if you have a setup that works well with the laptop camera; although it may be easier to position a phone. 

### Wired 
To use a wired connection, you need a way for your laptop to recognize your phone as one of your webcams. The best way to accomplish this is with Iriun Webcam (https://iriun.com/), which you install on both your smartphone and laptop. Then, execute `transit_plot_wired.py`

### Wireless (Android Only) 
The wireless connection has more limitations, but can be convinient if the circumstances are correct. This option uses the IP Webcam app that is only available on Android devices. The app will stream the video feed to an IP address, which you will need to copy and paste as the "url" variable in the `transit_plot_wireless.py script`. You will also need to have both devices connected to the same Wifi network for this to work. 
