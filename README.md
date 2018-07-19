# stft.js
A Javascript Short-Time Fourier Transform Implementation for audio applications.

Depends on [dsp.js](https://github.com/corbanbrook/dsp.js).

Use constructor for configuring with the desired stft parameters, then use *analyze* for analysis applications (process a buffer in one go) or *overlapAdd* for real-time spectral processing. For an example of the latter, see https://github.com/g-roma/twowaymixer. 

In both cases you supply a function (*processFunc*) that will be passed the real and imaginary parts of the frequency domain array for each frame.
