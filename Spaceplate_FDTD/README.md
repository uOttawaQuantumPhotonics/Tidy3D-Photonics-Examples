# Simulating a multilayer optical spaceplate with Tidy3D

**Status:** The tutorial notebook is in development and will be added here when it is ready.

How much free-space propagation can a thin stack of dielectric layers reproduce? A spaceplate gives each plane-wave component of an incident beam an angle-dependent phase shift. Over its operating angular range, these phase shifts reproduce the beam evolution expected after propagation through an effective distance $d_{\mathrm{eff}}$. The compression factor $R = d_{\mathrm{eff}}/d$ compares this distance with the physical thickness $d$ of the multilayer.

## Tutorial scope

The tutorial uses finite-difference time-domain (FDTD) simulations in Tidy3D to study four multilayer spaceplates near 1550 nm. Two use Fabry–Pérot cavities (FPC1 and FPC2), and two use aperiodic layer sequences obtained by gradient descent (GD1 and GD2).

- Build the four multilayer stacks and identify their resonances from the simulated transmission spectra.
- Map the electric field inside the Fabry–Pérot devices at a selected resonance.
- For FPC1, calculate how transmitted power varies with incidence angle at a fixed wavelength.
- For FPC2, compare the transmitted field with an empty-space reference and use its angular phase dependence to estimate the effective propagation distance and compression factor.

## Authors

Lucie Wang, Yaryna Mamchur, Manuel F. Ferrer-Garcia, and Jeff S. Lundeen  
Nexus for Quantum Technologies, Department of Physics, University of Ottawa

## Related publication

The device designs and experimental measurements are described in R. Hogan *et al.*, “Experimental demonstration of high space compression by optical spaceplates,” *Nature Communications* **17** (2026). [Read the paper](https://doi.org/10.1038/s41467-026-71500-1).

