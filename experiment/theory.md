
## Topic Description  
Photon–semiconductor interactions form the basis of optoelectronic devices such as LEDs, lasers, and solar cells. These interactions involve:  

- **Photon absorption**: The process by which photons transfer their energy to electrons, generating electron–hole pairs in the semiconductor.
- **Recombination**: The process by which electrons and holes combine, releasing energy either as light (radiative) or heat (non-radiative).
- **Bandgap type dependence**: The efficiency and mechanism of photon interaction depend critically on whether the semiconductor has a direct or indirect bandgap.

### Fundamental Processes

- **Absorption**: Photons with energy greater than or equal to the bandgap  
  $$ h\nu \geq E_g $$  
  can excite electrons from the valence band to the conduction band, creating electron-hole pairs.  

- **Emission**: Excited carriers recombine to release energy either as light (luminescence) or heat (non-radiative). The emission wavelength is determined by the bandgap energy: $\lambda = \frac{hc}{E_g}$.

- **Direct vs. Indirect bandgap**: In direct bandgap semiconductors (e.g., GaAs, InP), the conduction band minimum and valence band maximum occur at the same momentum value, enabling efficient radiative recombination. In indirect bandgap semiconductors (e.g., Si, Ge), momentum conservation requires phonon participation, making radiative recombination less efficient.  

<p><img src="images/gaptransitions.png" ></p> 

---

## Photon Absorption  

The **absorption coefficient** $ \alpha(h\nu) $ quantifies how strongly a material absorbs light of photon energy $ h\nu $. It determines the penetration depth and absorption length of light in the semiconductor.

The intensity of light decreases exponentially with distance according to Beer-Lambert law:  

$$ I(x) = I_0 e^{-\alpha x} \tag{5.11.1} $$  

where $I_0$ is the incident intensity and $x$ is the penetration depth.

### Direct Bandgap Semiconductors

For **direct bandgap semiconductors** (e.g., GaAs, InP, GaN), vertical transitions dominate and the absorption coefficient varies as:  

$$ \alpha(h\nu) \propto \sqrt{h\nu - E_g} \tag{5.11.2} $$  

This square-root dependence results from the joint density of states for direct transitions. Direct bandgap materials have high absorption coefficients ($\sim 10^4 - 10^5$ cm$^{-1}$) near the band edge.

### Indirect Bandgap Semiconductors

For **indirect bandgap semiconductors** (e.g., Si, Ge), phonon-assisted transitions are required to conserve momentum:  

$$ \alpha(h\nu) \propto (h\nu - E_g \pm E_{ph})^2 \tag{5.11.3} $$  

where $E_{ph}$ is the phonon energy involved in the transition. The ± sign indicates phonon absorption (+) or emission (−). Indirect bandgap materials have lower absorption coefficients ($\sim 10^2 - 10^3$ cm$^{-1}$), requiring thicker layers for efficient absorption.  

<p><img src="images/tran.jpg" ></p> 
---

## Emission Processes  

When carriers recombine, photons may be emitted through various mechanisms:  

- **Spontaneous Emission (Luminescence):** Random, independent photon emission when an electron in the conduction band recombines with a hole in the valence band without external stimulation.
- **Stimulated Emission:** An incoming photon triggers emission of another photon with identical phase, direction, energy, and polarization — the fundamental principle behind lasers and optical amplifiers.
- **Non-radiative Recombination:** Energy is released as heat through phonons instead of photons, reducing device efficiency.

<p><img src="images/emission.jpg" ></p>
<p><img src="images/stimulated_emission.png" ></p>

### Rate of Spontaneous Emission

The rate of spontaneous radiative recombination in semiconductors is given by:

$$ R_{sp} = B(np - n_i^2) \tag{5.11.10} $$

where:
- $n$ and $p$ are the electron and hole concentrations
- $n_i$ is the intrinsic carrier concentration
- $B$ is the bimolecular recombination coefficient (also called radiative recombination coefficient)

This relation shows that net recombination occurs only when $np > n_i^2$ (excess carrier condition). Under thermal equilibrium, $np = n_i^2$ and $R_{sp} = 0$.

### Types of Luminescence  
- **Fluorescence:** Rapid luminescence with short carrier lifetime ($\sim$ ns), ceasing almost immediately when excitation stops.
- **Phosphorescence:** Delayed luminescence with long carrier lifetime ($\sim$ µs–ms), persisting after excitation due to metastable trap states.  

---

## Light Amplification and Laser Action  

Under **population inversion** (when $N_2 > N_1$, where $N_2$ and $N_1$ are upper and lower state populations), stimulated emission dominates over absorption, leading to light amplification. This is a non-equilibrium condition achieved through external pumping.

### Requirements for Laser Operation

Laser (Light Amplification by Stimulated Emission of Radiation) operation requires:  
1. **Population inversion**: More carriers in the excited state than in the ground state  
2. **Optical feedback**: A cavity with mirrors providing resonance at specific wavelengths  
3. **Sufficient gain**: Optical gain must exceed all losses (absorption, scattering, mirror transmission)

The threshold condition for lasing is:
$$ G \cdot L \geq \alpha_{loss} \cdot L + \frac{1}{2}\ln\left(\frac{1}{R_1 R_2}\right) $$

where $G$ is the gain coefficient, $L$ is the cavity length, $\alpha_{loss}$ represents internal losses, and $R_1$, $R_2$ are mirror reflectivities.  


---

## Key Equations Summary

**Beer-Lambert Absorption Law:**  
$$ I(x) = I_0 e^{-\alpha x} \tag{5.11.4} $$  

**Direct Bandgap Absorption Coefficient:**  
$$ \alpha(h\nu) \propto \sqrt{h\nu - E_g} \tag{5.11.5} $$  

**Indirect Bandgap Absorption Coefficient:**  
$$ \alpha(h\nu) \propto (h\nu - E_g \pm E_{ph})^2 \tag{5.11.6} $$  

**Spontaneous Emission Rate:**  
$$ R_{sp} = B(np - n_i^2) \tag{5.11.7} $$  

**Stimulated Recombination Rate:**  
$$ R_{\text{stimulated}} \propto B_{21}\,\rho(h\nu) \tag{5.11.8} $$  

**Optical Gain:**  
$$ G = \sigma_{\text{stim}} (N_2 - N_1) \tag{5.11.9} $$  

---
