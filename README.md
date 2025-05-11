## Classification of Radio Signals into Pulsars and Non Pulsars using k-Nearest Neighbours 🌠


A **pulsar** is a highly magnetized rotating neutron star that emits beams of electromagnetic radiation out of its magnetic poles.

Since pulsars rotate rapidly, the emission of a pulsar forms a pattern that repeats periodically. This emission pattern varies slightly with each rotation and is unique for a pulsar. Therefore, the signal from a pulsar is averaged over many rotations giving us the fold/integrated profile of a pulsar. Since the Integrated pulse profile is unique to a pulsar it is also called a pulsar’s fingerprint(Lyon, 2016).

In practice, most signals are due to radio frequency interference (RFI) and noise. Without additional information, all “candidate” signals collected by a radio telescope could be classified as pulsars. To help differentiate pulsars and non-pulsar signals, we also use the DM-SNR (Dispersion Measure vs Signal to Noise Ratio) curve for the signal(Eatough et al., 2020).

**Our question is: Given a new candidate signal, can we classify it as a pulsar or non-pulsar?**

We use the HTRU2 data set available at the UCL machine learning repository. In this dataset, we use characteristics such as mean, standard deviation, excess kurtosis, and skewness for both the integrated profile and DM-SNR curve of a signal. For each candidate signal, there is a class label which classifies the detection as either a pulsar(1) or non-pulsar(0); a human annotator has classified the signals.
