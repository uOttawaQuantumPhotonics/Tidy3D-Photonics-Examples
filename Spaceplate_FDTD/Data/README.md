# Multilayer spaceplate design data

This folder holds the layer-thickness data used in the *Simulating a multilayer optical spaceplate with Tidy3D* tutorial. The notebook is under development.

The tutorial demonstrates three ways to define a multilayer stack. It generates the Fabry–Pérot designs (FPC1 and FPC2) from layer patterns, defines GD1 with a list of thicknesses in the notebook, and reads the layer sequence for the GD2 example from a CSV file.

## Layer-thickness file

The notebook reads the CSV column named `Layer Thicknesses`. Each row gives the physical thickness of one layer in micrometres (µm). Rows follow the order in which light encounters the layers. The notebook assigns the high-index material to the first layer and alternates between low and high index for each subsequent layer. Preserving the row order is therefore essential to reconstructing the device.

## Using the data

In the notebook’s **GD2 Parameters** cell, set `spreadsheet` to the path of the CSV file in this folder. A relative path is resolved from the notebook’s working directory. Keep `thickness_column="Layer Thicknesses"` and `unit_scale=1` when using thicknesses in micrometres.
