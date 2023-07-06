# ICR - Identifying Age-Related Conditions
Machine Learning to detect health conditions with measurements of anonymous characteristics.
# Context

They say age is just a number but a whole host of health issues come with aging. From heart disease and dementia to hearing loss and arthritis, aging is a risk factor for numerous diseases and complications. The growing field of bioinformatics includes research into interventions that can help slow and reverse biological aging and prevent major age-related ailments. Data science could have a role to play in developing new methods to solve problems with diverse data, even if the number of samples is small.

Currently, models like XGBoost and random forest are used to predict medical conditions yet the models' performance is not good enough. Dealing with critical problems where lives are on the line, models need to make correct predictions reliably and consistently between different cases.

Founded in 2015, [competition host InVitro Cell Research](https://invitrocellresearch.com/), LLC (ICR) is a privately funded company focused on regenerative and preventive personalized medicine. Their offices and labs in the greater New York City area offer state-of-the-art research space. InVitro Cell Research's Scientists are what set them apart, helping guide and defining their mission of researching how to repair aging people fast.

in this project, i worked with measurements of health characteristic data to solve critical problems in bioinformatics. Based on minimal training.

More information about Kaggle competition [here](https://www.kaggle.com/competitions/icr-identify-age-related-conditions/data)

# Dataset Description
The competition data comprises over fifty anonymized health characteristics linked to three age-related conditions. Your goal is to predict whether a subject has or has not been diagnosed with one of these conditions -- a binary classification problem.

# Files and Field Descriptions
* **train.csv** - The training set.
    * `Id` Unique identifier for each observation.
    * `AB-GL` Fifty-six anonymized health characteristics. All are numeric except for `EJ`, which is categorical.
    * `Class` A binary target: 1 indicates the subject has been diagnosed with one of the three conditions, 0 indicates they have not.

* **test.csv** - The test set. The goal is to predict the probability that a subject in this set belongs to each of the two classes.
* **greeks.csv** - Supplemental metadata, only available for the training set.
    * `Alpha` Identifies the type of age-related condition, if present.
    * `A` No age-related condition. Corresponds to class 0.
    * `B`, `D`, `G` The three age-related conditions. Correspond to class 1.
    * `Beta`, `Gamma`, `Delta` Three experimental characteristics.
    * `Epsilon` The date the data for this subject was collected. Note that all of the data in the test set was collected after the training set was collected.

Original Submission [here](https://www.kaggle.com/code/alarchemn/the-importance-of-prob-calibration-cv-and-metrics)
