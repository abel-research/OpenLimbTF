# OpenLimbTF
An Open-Source transfemoral residual limb anatomic dataset

**DOI:** [![DOI](https://img.shields.io/badge/doi-10.1101/2024.11.27.24317622-brightgreen)](https://doi.org/10.1101/2024.11.27.24317622)
**Data License:** [![License](https://img.shields.io/badge/license-CC--BY--SA--4.0-green)](../main/DATA-LICENSE)
**Code License:** [![License](https://img.shields.io/badge/license-MIT-blueviolet)](../main/CODE-LICENSE)

There are over 5,000 new lower limb amputations every year in the UK, and a major challenge is rehabilitating people with amputations by enabling them to return to normal activities, using a prosthetic limb. However, the residual limb is not initially suited for supporting the loads associated with standing or walking, and discomfort is common. The production of an appropriate patient-specific prosthetic socket is key, and today this is designed as a work of sculpture, by a highly experienced prosthetist. 

Many patient anatomy, surgery and disease factors can influence the socket design; however, few researchers have access to volumetric medical imaging data required to perform biomechanical analysis of socket designs. 

OpenLimbTF is a resource which contains a statistical description of transfemoral amputated residual limbs based CT images from the New Mexico Decedent Individuals Database, USA. These descriptions include the external surface of the residual limb, the residual femur and hemipelvis  (Figure 1, below).

<p align="center">
  <img src="../main/abstract/Process.png" alt="Generating a transfemoral residual limb Statistical Shape Model from medical imaging data (1), segmented, aligned and registered (2) to produce a mean shape (3) and principal modes of shape variability (4) shown in anterior and lateral views, with associated variance %" width="600"/>
</p>

The Machine Learning method Principal Component Analysis (PCA) has been used to reduce the dimensionality of this anatomic dataset to generate a mean residual limb shape, and independent modes of shape variation (Figure 2, below). As such, the dataset describes the anatomic variation across the training dataset without including any identifiable representation of the individuals.

<p align="center">
  <img src="../main/abstract/ModesTF.png" alt="Creating example virtual individuals from the mean limb shape and its variation in the first two principal modes" width="400"/>
</p>

This dataset is intended to allow the research community to perform more statistically robust prosthetic biomechanics research, without the costs, inconvenience, and risk of putting our relatively small community of eligible research participants through medical imaging.

The first OpenLimbTF Version-2025-05 is based upon 7 training datasets, 1 female and 6 male of a variety of ethnicities (5 White European/US, 2 Hispanic). 

You can download the model's mean shape, and virtual patient shapes covering 95% of training dataset variation in residual limb length and soft tissue bulbous-conical profile, as .stl files. These are normalised to the fractional intact length of the femur, so should be scaled up to the desired intact femur length.

For more detailed descriptions of the dataset and statistical testing behind it, please refer to the publication linked below.

How to acknowledge
------------------

OpenLimbTF has not yet been presented or published, so for now please cite as:

K. Pasternak, F.E. Sunderland, A.J. Sobey, the OpenLimb Group, P.R. Worsley, A.S. Dickinson (2025), OpenLimbTF, a Transfemoral Residual Limb Shape Model for Prosthetics Simulation and Design: creating a statistical anatomic model using sparse data. [https://github.com/abel-research/openlimbTF](https://github.com/abel-research/OpenLimbTF).

OpenLimb Group Membership
--------

At the time of writing, the OpenLimb Group includes:
- Dr Jennifer Bramley, Prof Alex Dickinson, Prof Cheryl Metcalf, Karol Pasternak, Prof Adam Sobey, Dr Joshua Steer, Fiona Sunderland, and Prof Peter Worsley (University of Southampton, UK),
- Dr Rami Al-Dirini (Flinders University, Australia),
- Dr Reza Safari (University of Derby, UK),
- Dr Graci Finco (The University of North Texas, USA),
- Dr Ziyun Ding (University of Birmingham, UK),
- Prof Anthony Bull, Dr Diana Toderita and Dr David Henson (Imperial College London, UK), and
- Dr Arjan Buis (University of Strathclyde, UK).

Funding
--------

The research behind this dataset was funded by the following organisations:
- the Royal Academy of Engineering (RAEng), UK (grant no. RF/130 (A Dickinson))
- the Alan Turing Institute, UK (grant no. EP/N510129/1 (A Dickinson, A Sobey))
- the US National Institute of Justice (grant no. 2016-DN-BX-0144 (The Free Access Decedent Database))

Ethical Approvals
--------

This secondary data analysis work was granted ethical approval by the University of Southampton's Ethics and Research Governance Office (ERGO 65748.A2)

Original data collection work was granted ethical approval by the following committees:
- 

License
--------

This dataset uses a Creative Commons Attribution Share Alike 4.0 International license, which can be found [here](../main/LICENSE)
Share Alike means that if you remix, transform, or build upon the dataset, you must distribute your contributions under the same license.
