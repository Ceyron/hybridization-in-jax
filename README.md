# Hybridization in JAX with AD

I was invited to give a lecture and practical sessions at the [Workshop on
Machine Learning and Automatic Differentiation in `JAX` for Scientific Computing
](https://majsc2026.pages.math.unistra.fr/) hosted by the University of
Strasbourg in June 2026. For this, I presented a lecture on hybridization (i.e.,
how to marry neural networks and numerical solvers) as well as a practical
session on using the [Exponax](https://fkoehler.site/exponax/) solver suite in
JAX for solving PDEs (concretely the Kolmogorov Flow), data assimilation,
inverse problems, and to build neural-hybrid correctors leading to a simplified
reproduction of the influential [ML-accelerated CFD paper by Kochkov et al.](https://www.pnas.org/doi/10.1073/pnas.2101784118). Thank you for having me!

## Recordings

Recording of the lecture:

[![Link to the lecture recording](https://img.youtube.com/vi/carwzAOfuPE/0.jpg)](https://www.youtube.com/watch?v=carwzAOfuPE)

Recording of the "zeroth" practical session on getting started with Exponax by solving the 2D Navier-Stokes Kolmogorov Flow:

[![Link to the "zeroth" practical session recording](https://img.youtube.com/vi/I7ilrh6tbVc/0.jpg)](https://www.youtube.com/watch?v=I7ilrh6tbVc)

Recording of the first practical session on data assimilation and inverse problems:

[![Link to the first practical session recording](https://img.youtube.com/vi/Tb3n52Ka4GM/0.jpg)](https://www.youtube.com/watch?v=Tb3n52Ka4GM)

Recording of the second practical session on building neural-hybrid correctors:

[![Link to the second practical session recording](https://img.youtube.com/vi/g1guv-fkIrQ/0.jpg)](https://www.youtube.com/watch?v=g1guv-fkIrQ)

## Material Overview

This repository contains all my material for the lecture and practical session I gave at the [ML & AD in JAX](https://majsc2026.pages.math.unistra.fr/index.html) workshop at the University of Strasbourg in June 2026.

In the notebooks, the videos have been removed to save space.

See also [this Hugging Face repo](https://huggingface.co/datasets/ceyron/jax-ad-workshop), which contains the datasets for the second exercise.

### Getting Started

0. Install the [Colab Extension for VS Code](https://marketplace.visualstudio.com/items?itemName=Google.colab) and register with your Google account.
1. `cd` into your preferred directory and then clone the repository `git clone https://github.com/Ceyron/hybridization-in-jax.git`
2. Open the folder with VS Code, open a notebook, then under kernel click on Colab <img width="2400" height="734" alt="image" src="https://github.com/user-attachments/assets/557efd61-6445-499b-a7ad-3c11f4496561" />
3. Follow the steps, make sure to select `GPU` and select the (free) `T4` GPU
4. It may take ~15 seconds for the server to spin up, then in the dropdown select the Python runtime <img width="2404" height="618" alt="image" src="https://github.com/user-attachments/assets/dbb60e61-895a-4f23-addc-76ef101d2e61" />
5. Then it may take another ~15 seconds for the runtime to connect. Afterward, you can use the notebook natively.
6. Important! The runtime is on the Colab servers, hence you will have to install all pip dependencies and download datasets. In the notebooks, you will find commented-out bash commands for this.

Some nice trick: If you want to monitor GPU usage, click on the Colab entry in the top bar and then spawn a terminal on the remote machine .<img width="2402" height="680" alt="image" src="https://github.com/user-attachments/assets/75d866ec-0a8d-411c-9d39-fb0624b283b5" />. In this terminal, run `uvx nvitop`.


