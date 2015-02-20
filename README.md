# pheno_screen

All functions to be used in phenotypic screens.

* QC : Quality control measures

	- `cv_check`: calculates the coefficient of variation if given a column of measurements, and a column with which to group the elements by. Produces a dataframe containing the CV for each element of the group. 

	- `cv_plot`: similar to cv_check, but produces a graph of coefficient of variation (y) against group (x) instead of a data frame. Less flexible than manually calling plot on `cv_check` results. Optional arguments to produce plot in ggplot, add a connecting line between points or rotate x-axis labels.

	- `z_factor.R`: calculates a z-factor or z` factor to assess how robust the difference is between groups. A z-value of 0.5 equates to a difference of 12 standard deviations between the two groups.

	- `poc.R`: 'Percentage Of Control', measures compound activity as a percentage of a positive control.

	- `npi.R`: 'Normalised Percentage inhibition', for use in antagonism assays. Calculates the percentage inhibition normalised against the positive and negative controls.

	- `ssmd.R`: 'Strictly standardised mean difference', calculates the difference between two groups.

	- `mad.R`: 'Median Absolute Deviation': *incomplete*

	- `b_score.R` *incomplete*
