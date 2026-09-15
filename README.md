# Computational Projects

A collection of my computational physics projects, exploring collective motion and acoustics through Python simulations and data analysis.

## Projects

### Vicsek Model: Collective Motion

[Open the notebook](vicsek-model/viscek-model.ipynb)

A two-dimensional simulation of self-propelled particles moving at a constant speed. Particles align with nearby neighbors, with random angular noise and periodic boundaries. A live quiver plot shows the motion, and the notebook records observations from varying the interaction radius and noise strength.

Based on [Vicsek et al., *Novel Type of Phase Transition in a System of Self-Driven Particles* (1995)](https://doi.org/10.1103/PhysRevLett.75.1226).

### Acoustics: Fourier Analysis and Timbre

[Open the notebook](acoustics/Project/acousticsproject.ipynb) · [Read the PDF](acoustics/Project/acousticsproject.pdf)

A project with Aaron comparing real bassoon recordings, MIDI bassoon samples, and generated tones. Fast Fourier transforms reveal how fundamental frequencies and overtone strengths shape the sounds' timbre. The project includes the audio recordings used in the analysis.

The `acoustics/noneed/` folder contains earlier experiments and supporting files; `acoustics/Project.zip` is the existing project archive.

## Running the Notebooks

Use Python 3 with Jupyter and the following packages:

```sh
python -m pip install jupyterlab numpy matplotlib scipy pandas librosa ipympl
python -m jupyter lab
```

- **Vicsek model:** Open `vicsek-model/viscek-model.ipynb`, run the initialization cell to display the widget, then run the simulation cell. The animation uses `%matplotlib widget` and updates the existing plot without storing frame history.
- **Acoustics:** Open `acoustics/Project/acousticsproject.ipynb` and run the cells in order. Keep the notebook's working directory set to `acoustics/Project/` so its relative audio paths resolve.
