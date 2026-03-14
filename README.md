The Jupyter Notebooks in this repository are associated with the 2026 HamSCI Workshop presentation “Introduction to Baseband Processing” by Phil Erickson, W1PJE, Bill Liles, NQ6Z, and Ethan Miller, K8GU.

It is advised that one view the video recording of the tutorial at the HamSCI meeting, and examine the presentation slide, before exploring the Notebooks. The slides and the video will be posted on HamSCI.org at a later date after the presentation. This README will be updated when those items are available.

(Those not familiar with Jupyter Notebooks can consult available online references for tutorials on editing and executing Notebook code - e.g. https://www.codecademy.com/article/how-to-use-jupyter-notebooks .)

Note: bandpass can have multiple definitions in the technical and academic literature. For these Notebooks, the term bandpass is defined as applying to in-phase/quadrature (IQ) complex signals with a center frequency of 0 Hz.

Notebooks provided cover several areas relevant to bandpass signal processing.

    Notebooks are provided that implement functions for common transformation tasks applied to baseband signals. Symmetry/Asymmetry refers here to the frequency domain shape of the filter.

    Symmetric low pass filter
    Symmetric high pass filter
    Asymmetric band pass filter
    Asymmetric notch filter
        Asymmetric notch filter, with one notch
        Asymmetric notch filter, with multiple notches

    Notebooks are provided to extract information content from baseband signals.
        Amplitude modulation (AM) signal demodulation
        Narrowband frequency modulated (NBFM) signal demodulation

    Notebooks are provided to translate signal information content in frequency.
        Conversion of pass band signals to baseband
        Conversion of baseband signal to pass band

When running code, the Notebooks are set up to open the plots in separate windows. This allows for zooming and other interactive manipulation of the plots. If inline plotting is desirable instead, simply remove, or do not execute, the second cell that has the command “%matplotlib qt” in it.

For each notebook, the top cells have “import” statements that add modules external to the Notebook. The user is responsible for making sure these modules are installed before executing the code. Please consult standard python references for instructions on how to find and install these.

Note that due to time constraints, some Notebooks - specifically those covering asymmetric notch filters with multiple notches, NBFM demodulation, conversion of pass band signal to baseband, and conversion of baseband signal to pass band - are not discussed in the presentation. These are provided as an exercise for the user.

Example “wav” format files (RIFF (little-endian) data, WAVE audio, Microsoft PCM, 16 bit) providing signal inputs for the AM demodulation and NBFM demodulation Notebooks are included. The user should be aware that different software tools for saving IQ signal files from software defined radios (SDRs) can have different formats, even within “wav” format files. Accordingly, modification of code in these Notebooks might need to be changed, particularly in the file read cell, based upon the specific IQ wav file format used in recording the signal from a particular SDR or other digital source.
