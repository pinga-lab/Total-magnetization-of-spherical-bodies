# Estimation of the total magnetization direction of approximately spherical bodies

[Vanderlei C. Oliveira Jr.](http://fatiando.org/people/oliveira-jr/)<sup>1</sup>,
Daiana P. Sales<sup>1</sup>,
[Valéria C. F. Barbosa](http://lattes.cnpq.br/0391036221142471)<sup>1</sup>,
[Leonardo Uieda](http://www.leouieda.com/)<sup>1,2</sup>

<sup>1</sup>[*Observatório Nacional*](http://www.on.br/);
<sup>2</sup>[*Universidade do Estado do Rio de Janeiro*](http://www.uerj.br/)

This repository contains the manuscript and supplementary code
and data for the article
"Estimation of the total magnetization direction of approximately spherical
bodies"
submitted to the journal Nonlinear Processes in Geophysics.

The original submission and open peer-review of this article can be found at:
http://dx.doi.org/10.5194/npgd-1-1465-2014

The repository is archived in Zenodo: http://dx.doi.org/10.5281/zenodo.16191

## Abstract

We have developed a fast total-field anomaly inversion to estimate the
magnetization direction of multiple sources with approximately spherical
shape and known centres. Our method can be applied to interpret multiple
sources with different magnetization directions. It neither requires the
prior computation of any transformation like reduction to the pole nor the
use of regularly spaced data on a horizontal grid. The method contains
flexibility to be implemented as a linear or non-linear inverse problem,
which results, respectively, in a least-squares or robust estimates of the
components of the magnetization vector of the sources. Applications to
synthetic data show the robustness of our method against interfering
anomalies and errors in the location of the sources' centre. Besides, we
show the feasibility of applying the upward continuation to interpret
non-spherical sources. Applications to field data over the Goiás Alkaline
Province (GAP), Brazil, show the good performance of our method in estimating
geological meaningful magnetization directions. The results obtained for a
region of the GAP, near from the alkaline complex of Diorama, suggest the
presence of non-outcropping sources marked by strong remanent magnetization
with inclination and declination close to -70.35<sup>o</sup> and -19.81<sup>o</sup>,
respectively. This estimated magnetization direction leads to predominantly positive
reduced-to-the-pole anomalies, even for other region of the GAP, in the
alkaline complex of Montes Claros de Goiás. These results show that the
non-outcropping sources near from the alkaline complex of Diorama have almost
the same magnetization direction of that ones in the alkaline complex of
Montes Claros de Goiás, strongly suggesting that these sources have emplaced
the crust almost within the same geological time interval.

## Reproducing the results

The [IPython notebooks](http://ipython.org/notebook.html) located in the
`notebooks` directory of this repository
generate all synthetic data, results, and figures in this paper.
They the [Fatiando a Terra](http://fatiando.org) library
and libraries from the [Scipy ecosystem](http://scipy.org/)
to perform the calculations and generate figures.

You can view a static version of the notebooks without having to download or
install anything in the
[nbviewer](http://nbviewer.ipython.org/) web service:

http://nbviewer.ipython.org/github/pinga-lab/Total-magnetization-of-spherical-bodies/tree/master/notebooks/

Navigate to the folder containing the notebook you want to view and click on
the `.ipynb` file. You won't be able to run the code in this online version.

The method proposed in this paper is implemented in Fatiando a Terra version
0.3. You can
[view the code online](https://github.com/fatiando/fatiando/blob/v0.3/fatiando/gravmag/magdir.py#L29)
or download a copy from the official website.

### Getting the files

To actually run the code in the notebooks,
you'll need to have the files on your machine.
You can download a
[zip archive of this repository](https://github.com/pinga-lab/Total-magnetization-of-spherical-bodies/archive/master.zip)
to get everything.
You can also download the repository from Zenodo:
http://dx.doi.org/10.5281/zenodo.16191

### Installing the software

You'll need to install Python and the required libraries
to execute the IPython notebooks.
The easiest way to get Python and all libraries installed
is through the
[Anaconda Python distribution](http://continuum.io/downloads).
Be sure to select the **Python 2.7** version of Anaconda.
After you've installed Anaconda,
install the libraries by running the following command
in your terminal:

    conda install numpy scipy ipython ipython-notebook matplotlib mayavi imaging basemap pip

After Anaconda, you'll need to install the geophysics library
[Fatiando a Terra](http://www.fatiando.org).
You can do this by running the following command
in your terminal:

    pip install fatiando==0.3

See the
[documentation of Fatiando a Terra](http://fatiando.github.io/v0.3/install.html)
for more detailed instruction.

### Running the IPython notebooks

Once the software is installed, you must start an IPython notebook server to
run the code in the notebooks.
Do this by typing in a terminal (or `cmd.exe` in Windows):

    ipython notebook

This should open an Internet browser tab with a page to navigate your computers
folders.
Go to where you saved the `notebooks` folder on your computer and click on
the notebook file you want to run (the `.ipynb` files).
You can execute the code cells by clicking on one and typing `Shift+Enter`.
Be sure to execute the code cells in descending order to get the correct
results.
Some cells may take a long time to run.
