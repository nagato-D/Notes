+++
title = 'Note on Thin-Film Lithium Niobate'
date = 2023-10-15T17:08:36+08:00
draft = false
+++

**Author** Di Yu

## Overview
---
- [Overview](#overview)
- [Background](#background)
- [Advantages of Lithium Niobate](#advantages-of-lithium-niobate)
- [Traditional Waveguides on Bulky LN](#traditional-waveguides-on-bulky-ln)
- [Preparation of LN Thin Films](#preparation-of-ln-thin-films)
- [Etching Process for Thin-Film LN](#etching-process-for-thin-film-ln)
- [State of the Art](#state-of-the-art)
- [Lasers on Thin-Film LN](#lasers-on-thin-film-ln)
  - [Cover Page](#cover-page)
  - [Laser Design](#laser-design)
  - [Static Characterization (Transmission Spectra \& Power \& Linewidth)](#static-characterization-transmission-spectra--power--linewidth)
  - [Dynamical Characterization (Frequency Tuning)](#dynamical-characterization-frequency-tuning)
  - [Second Harmonic Generation](#second-harmonic-generation)
  - [Future Work](#future-work)
- [References](#references)

## Background
---
+ The successes of manufacturing **wafer-scale, high-quality thin films of LN-on-insulator (LNOI)** and breakthroughs in nanofabrication techniques have made high-performance integrated nanophotonic components possible.
+ With rapid development in the past few years, some of these thin-film LN devices, such as optical modulators and nonlinear wavelength converters, have already **outperformed** their legacy counterparts realized in bulk LN crystals.

## Advantages of Lithium Niobate
---
1. Broad transparency window, from 350 nm to 5 um;
2. Relatively large refractive index, ~2.2 at 1550 nm;
3. Large second-order nonlinear coefficients;
4. Large Pockels coefficient.

## Traditional Waveguides on Bulky LN
---
Traditional integrated LN devices are absed on low-index-contrast waveguides, normally formed by titanium (Ti) indiffusion or proton exchange in bulk LN. These devices have **weak mode confinement**, **large device footprints**, and **reduced nonlinear efficiencies**. Additionally, it is impossible to make tight bends in these diffusion-based LN waveguides, which prevents the realization of low-loss ring resonator. These limitations motivated the production of thin-film LN-on-insulator wafers.

<center><img src='figures/waveguides_bulky_LN.png' width=400></center>

## Preparation of LN Thin Films
---
The development and refinement of the "**Smart-Cut**" technology has emerged as the **standard technique for producing high-quality LN thin films**. The film is split from a high-quality bulk substrate through ion slicing and thermal annealing, and is bonded to an insulating substrate.

<center><img src='figures/smart-cut.png' width=600></center>

The use of ion slicing with direct wafer bonding, **large-scale single-crystalline LN thin films were demonstrated**. Currently, **LNOI wafers with sizes up to 6 inches have been made commercially available**.

## Etching Process for Thin-Film LN
---
Dry etching of LN had been notoriously difficult. Unlike most other integrated photonics platforms such as Si and silicon nitride, **a proper reactive ion-etching recipe was not available for LN**. Fluorine-based RIE can remove LN effectively by forming volatile, fluorinated niobium species. However, it alos forms lithium fluoride (LiF), which is non-volatile, and results in severe redeposition problems. LiF is highly resistive to further etching, and thus increases sidewall roughness and scattering loss.

Currently, **pure physical etching** with Ar ion plasma is among the **most popular dry etching approaches** for LNOI. There are a few challenges associated with pure physical etching.

+ Low etch selectivity $\rightarrow$ limited etch depth.
+ Redeposition $\rightarrow$ tilted sidewalls, angled in the 40-80 degree range.

## State of the Art
---
+ 6-inch LNOI wafers are now commercially available.
+ Devices with optical loss **< 0.1 dB/cm** has been produced in several groups.
+ Sidewall roughness results in **scattering loss**, the major contribution of optical loss.
+ LN-based ring resonator with a Q-factor of **$10^{7}$** has been demonstrated.
+ Thin-film LN-based EO modulators with bandwidth **> 100 GHz** operating at CMOS-compatible voltages have been realized.

## Lasers on Thin-Film LN
---
### Cover Page
<center><img src='figures/title.png' width=400></center>

**Overview**
+ Published in **Nature Communication** on Sep. 12, 2022.
+ Demonstrate a thin-film LN-based extended cavity laser, integrating with electric-optic modulator and periodically poled LN, enabling high-speed modulation/switching and second harmonic generation.

**Performance** 
+ **Tuning rate = $2 \times 10^{18}$ Hz/s**
+ Switching speed = 50 MHz
+ **Operation wavelength = 1580/790 nm**
+ Wavelength tunability = 10 nm
+ Output power = 4 mW/2 uW
+ Linewidth = 11 kHz

### Laser Design
<center><img src='figures/laser_design.png' width=600></center>

**Components**
+ RSOA: reflective semiconductor optical amplifier, providing optical gain.
+ Spot-size converter: improve the conversion efficiency by mitigating mode profile mismatch.
+ Phase shifter: high-speed electric-optic modulator, enabling frequency tuning.
+ PPLN: periodically poled LN for quasi-phase-matching, allowing frequency doubling and enabling two-color lasing.
+ EOM: high-speed electric-optic modulator, controlling the mode (mis-)matching in the Vernier cavity, enabling high-speed switching.
+ Heater: thermo-optic modulator, providing broad-band modulation.
+ Loop mirror: Sagnac mirror with a reflectivity of 30%. 

### Static Characterization (Transmission Spectra & Power & Linewidth)
<center><img src='figures/static_characterization.png' width=600></center>

+ (a) LIV curve, maximal laser **output power ~4 mW**.
+ (b) Straight coupling suppresses multi-mode lasing, while pulley coupling features high coupling efficiency in a broad band.
+ (c) Characterization of thermo-optic modulation, **wavelength tuning range ~20 nm**.
+ (d-e) Setup and results of noise characterization. **Delayed self-heterodyne measurement: lienwidth = 15 kHz; Correlated delayed self-heterodyne phase noise characterization: linewidth = 11 kHz**.

### Dynamical Characterization (Frequency Tuning)
<center><img src='figures/dynamical_characterization.png' width=600></center>

+ (a) Time-frequency spectrogram. Upper: frequency spectra of laser output versus time; Lower: **relative nonlinear deviation of the laser output (< 10%)**.
+ (b) Same as above, but with a **lower driving signal amplitude** ($V_{P} = 2V$), the **nonlinear deviation becomes lower**.
+ (c) Tuning efficiency (tuning range divided by driving signal amplitude). It remains almost constant when increasing the modulation speed until ~1 GHz, demonstrating **great linearity**.
+ (d) Frequency tuning rate versus modulation speed. It remains linear until modulation speed = 1 GHz/**frequency tuning rate = 2 EHz**.
+ (e) Time-frequency spectrogram. The laser output remains almost constant (relative variation < 10%) during the frequency tuning.
+ (f) High-speed on-off switching. Upper: laser output power; Lower: driving elcectrical signal. **50 MHz switching speed is recorded**.
+ (g) High-speed mode switching.

### Second Harmonic Generation
<center><img src='figures/SHG_characterization.png' width=600></center>

+ (a) Schematic of second harmonic generation.
+ (b) Optical image of the coupling port, visible light spot observed.
+ (c) Power spectral density of the laser output in the telecom/visible band, **demonstrating the two-color lasing** at wavelength 1581/790 nm.
+ (d) **Quadratic dependence of visible laser power on telecom laser power**. This is a feature of second harmonic generation.
+ (e) High-speed on-off switching of the two-color lasing.

### Future Work
+ Combine EO frequency modulation and intensity modulation by varying the current, enabling **fully integrated optical arbitrary waveform generator**.
+ Optimize the quality factors of the resonators to support much **higher speed modulation**.
+ Trough cascaded sum frequency generation, shorter wavelength at green or blue can be achieved, enabling lasing in a **broader spectrum range**.

## References
---
1. Zhu, Di, et al. "Integrated photonics on thin-film lithium niobate." Advances in Optics and Photonics 13.2 (2021): 242-352.
2. Li, Mingxiao, et al. "Integrated pockels laser." Nature communications 13.1 (2022): 5344.