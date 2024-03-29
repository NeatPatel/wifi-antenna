![](https://github.com/NeatPatel/wifi-antenna/blob/main/images/bi-quad_antenna.jpg?raw=true)

## Introduction:
Are you tired of weak Wi-Fi signals limiting your Internet access? One effective solution is to upgrade your router's antenna. In this blog post, I'll guide you through the process of designing and building your own Bi-Quad antenna. With just a few materials and some basic tools, you can significantly enhance your Wi-Fi coverage and enjoy faster Internet speeds.

### What are antennas and how do they work?
Antennas are devices that can be used to send or receive signals in the form of Electromagnetic Waves. Generally a Wi-Fi router antenna will not require any power, and will just intercept signals by catching EM (Electro-Magnetic) radiation and giving the input to the router to process. 

The interception of signals is possible because of something known as "induced current", where when a straight wire has current running through it, electromagnetic waves will begin to generate around it, called an induced B field (Magnetic field). 
  - This process works the other way around, and allows for electromagnetic fields existing around antennas to generate currents within the antenna. This process results in a current that can be sent as a signal to the router.

## Step 1: Gather Your Materials
Before diving into the construction process, make sure you have all the necessary materials on hand. You'll need:

- SMA-Male Connector, with a coaxial cable cut to around 6-7cm
- 8 gauge Copper wire in 1m length
- Soldering iron and solder
- Wire cutter/stripper
- Measuring tape

> Note: it is very important to have an SMA-Male connector, because this is what is used to connect to the router itself!

## Step 2: Understanding the Bi-Quad Antenna Basics
A Bi-Quad antenna consists of two copper wire square elements arranged in a cross configuration. This design allows for increased signal strength and improved directional coverage compared to standard antennas. All sides of each element are a quarter-wavelength long, making them resonate with the desired frequency of WI-FI, which is 2.45 GHz. 

This occurs because a quarter-wavelength is a close multiple to the desired frequency such that the signals picked up will make a maximum current at one end of the side, and a minimum at the other side. This together also allows for even propagation of the EM wave, rather than uneven propagation from something such as a 11/12 wave antenna.

## Step 3: Calculate Element Lengths
To achieve optimal performance, we'll need to find the length of the antenna element sides to find the quarter-wavelength desired frequency. Since the frequency is 2.45 GHz, we can use the following formula to calculate the wavelength:

$$\lambda = {c \over f}$$

Where c is the speed of light (since this is how fast radio waves travel), or approximate $3.0 \times 10^8 {m \over s}$ and $f$ is the frequency in Hertz (Hz), or $2.45 \times 10^9$ Hz for Wi-Fi

Calculating will yield a wavelength of about $0.1224$ m, or about $12.25$ cm for a wavelength, which needs to be divided by 4 to achieve an optimal quarter-wavelength. This means that each element's side needs to be about $0.0306$ m or $3.05$ cm long. Cut two pieces from the 1m length of copper wire with each segment being about 30 cm long.

## Step 4: Construct the Antenna Elements
Bend both of the wire segments into the shape as depicted in the image below, ensuring that the corners are at right angles:

![](https://github.com/NeatPatel/wifi-antenna/blob/main/images/biquad_size.png?raw=true)

When bending the wire into this shape, if any excess wire is remaining sticking out, use wire cutters to cut them off in order to keep the resonant frequency optimal.

## Step 5: Connecting to the Feed Point
Next, you'll need to connect the feed point where the coaxial SMA-Male Connector cable connects to the antenna. In order to do this, first solder together the two Bi-Quad elements.

The result should look this:

![](https://github.com/NeatPatel/wifi-antenna/blob/main/images/biquad_cross.jpg?raw=true)

Now, strip the insulation from the coaxial cable and solder the inner conductor to the bi-quad combined cross. The result should look like the antenna in the image at the beginning.

## Step 6: Test and Fine-Tune
Once the antenna is assembled, it's time to test its performance. Mount the antenna in a clear, elevated location and connect it to your Wi-Fi router using the coaxial cable. Use a Wi-Fi analyzer app or software to measure signal strength and coverage, such as [this nirsoft service](https://www.nirsoft.net/utils/wifi_information_view.html). If necessary, adjust the antenna's position or element lengths to optimize performance.

## Conclusion:
Now you have created your own Bi-Quad antenna and enhanced your Wi-Fi signal strength and coverage! With your effort and creativity, you can now enjoy faster internet speeds and a more reliable connection throughout your home or office. Say goodbye to Wi-Fi dead zones and hello to seamless browsing, streaming, and online gaming!
