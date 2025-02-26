# Protein signaling project

### Machine Learning and Causal Inference. MSc in Data Science Methodology. Barcelona School of Economics.

Project idea contributed by Alessandro Mascaro (UPF), based on an initial proposal by Sara
Magliacane (University of Amsterdam).

## Description

In this project you will conduct a causal discovery analysis of data collected
 by the study of Sachs et al. (2005), where the concentration of 11 key
[phosphorylated proteins](https://en.wikipedia.org/wiki/Protein_phosphorylation)
was measured by [flow cytometry](https://en.wikipedia.org/wiki/Flow_cytometry)
in human [peripheral blood lymphocytes](https://en.wikipedia.org/wiki/Peripheral_blood_lymphocyte),
across different conditions. The work of Sachs et al. (2005) shows how causal
discovery methods can recover known causal relationships in cellular signaling
networks from flow cytometry data generated with different molecular
interventions. For the purpose of this project, you may focus the analysis in
the following subset of the interventions explored in Sachs et al. (2005):

| Stimulation                    | Targets:                            |
|--------------------------------|-------------------------------------|
| α-CD3, α-CD28                  | Baseline condition, no intervention |
| α-CD3, α-CD28, AKT inhibitor   | AKT                                 |
| α-CD3, α-CD28, G0076           | PKC                                 |
| α-CD3, α-CD28, Psitectorigenin | PIP2                                |
| α-CD3, α-CD28, U0126           | MEK                                 |
| α-CD3, α-CD28, LY294002        | AKT                                 |

In this GitHub repo you will find a CSV file for each of the previous
experimental conditions, where each row corresponds to measurements taken from
individual cells under the corresponding condition.

Using the R packages [pcalg](https://cran.r-project.org/package=pcalg),
[BCDAG](https://cran.r-project.org/package=BCDAG), and the code provided as
additional material during the course, you can run different causal discovery
algorithms. In particular:

1. Run one or more algorithm for causal discovery from observational data such
   as PC, GES or Bayesian equivalents, on what we consider here as
   observational data, the baseline condition dataset.

2. Run the same causal discovery algorithm(s) on the dataset obtained by
   merging all the datasets from the different experimental conditions.

3. Run one or more algorithms for causal discovery from observational and
   experimental data, such as GIES, IGSP and Bayesian equivalents, specifying
   the targets of interventions indicated in the table above.

4. Compare the results of the different causal discovery algorithms, and in
   comparison with the results reported in Sachs (2005), try to figure out
   which better matches the underlying biology;

## Submission procedure

This project has to be submitted using
[GitHub Classroom](https://classroom.github.com). This means that you should
have cloned the GitHub repo of this project from the organization account for
MLCI https://github.com/mlci25 using the submission link provided through
Google Classroom.

Once you have cloned this GitHub repo, then you can work on it in your local
disk and _push_ your changes whenever you like, but make sure that you have
pushed the last version of your assignment before the deadline; consult the
Google Classroom if your are unsure about the deadline. There is no _submit_
button or any other specific submission procedure or action than just pushing
your changes to your GitHub assignment repo. When correcting the project, the
version available at the deadline will be retrieved. If the last update to the
repo is posterior to the deadline, then the mark of the assignment will have a
penalty.
