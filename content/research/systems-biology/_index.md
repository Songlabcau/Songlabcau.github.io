+++
# A Demo section created with the Blank widget.
# Any elements can be added in the body: https://wowchemy.com/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "blank"  # See https://wowchemy.com/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
# weight = 200  # Order that this section will appear.

title = "Systems Biology"
subtitle = ""

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "1"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
  # color = "navy"

  # Background gradient.
  gradient_start = ""
  gradient_end = ""

  # Background image.
  # image = "image.jpg"  # Name of image in `static/media/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.
  # image_size = "cover"  #  Options are `cover` (default), `contain`, or `actual` size.
  # image_position = "center"  # Options include `left`, `center` (default), or `right`.
  # image_parallax = true  # Use a fun parallax-like fixed background effect? true/false

  # Text color (true=light or false=dark).
  text_color_light = false

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "20px", "0"]

[advanced]
 # Custom CSS.
 css_style = ""

 # CSS class.
 css_class = ""
+++


   Rapid advances in high-throughput genomic technology have enabled biology to enter the era of ‘Big Data’ (large datasets). The plant science community not only needs to build its own Big-Data-compatible parallel computing and data management infrastructures, but also to seek novel analytical paradigms to extract information from the overwhelming amounts of data. Machine learning offers promising computational and analytical solutions for the integrative analysis of large, heterogeneous and unstructured datasets on the Big-Data scale, and is gradually gaining popularity in biology. Our lab also working on developing machine learning models for data mining in plants, and the ultimate goal is to construct a Big-Data virtual environment for the plant research community. In a recent review in the journal TRENDS in PLANT SCIENCES, we systematically introduce some basic concepts and models for machine learning in plants.
   {{< figure src="Systems_Biology.png" width="100%" >}}
   To explain the basic machine-learning terms and procedures for building a machine-learning system, we demonstrate the use of a supervised machine-learning method to discover genes responsive to salt stress and recommend high-priority candidate genes for phenotypic screening experiments (Figure I). The raw data are composed of 22 000 genes (examples) probed with an Affymetrix microarray whose expression values were profiled at six time points over a 24-h period, while root tissue was subjected to salt treatment. The raw data were first preprocessed by normalization to remove technical variations, imputation to replace missing values, and the transformation of six time-point values to 33 numeric statistics (attributes) to characterize the degree of expression change. Then, the clean dataset was converted to an input matrix of 22 000 genes in rows and 33 attributes in columns. The training set includes 900 known salt-related genes (labeled examples) as positive samples and 13 000 genes without expression change as negative samples. We treat this analysis as a classification problem, and use the random forest (RF) classifier (machine-learning model) to determine whether a gene was related to salt-induced response. The RF classifier builds a series of decision trees by resampling positive and negative samples, which are used to train and validate the final model. The n-fold cross-validation (evaluation metric) is used to assess the generation performance of the RF model (model validation and evaluation). The entire gene matrix is randomly split into n subsets; each of which keeps a roughly equal number of positive and negative samples. For each cross-validation, n–1 subsets are firstly merged into one dataset and then divided into two parts: the training dataset and the tuning dataset. Optimized parameters, at which the RF classifier has high precision and recall, are obtained by training on the training dataset and testing on the tuning dataset. The remaining subset is used as the testing dataset to evaluate the trained RF classifier’s prediction power by the ROC curve that plots the variation of TPR (y axis: true positive rate) versus FPR (x axis: false positive rate) at all possible prediction scores. After n rounds of cross-validation, an average AUC is calculated to represent the predictive power of the trained RF model. All the genes are ordered based on the priority scores assigned by the trained RF model. The genes with higher priority scores than a threshold are recommended as stress-related candidate genes, and the optimal threshold is determined when the maximal F-score is achieved. The recommended high-priority candidate genes with available Salk transfer DNA (T-DNA) mutation lines are functionally tested by phenotypic screening experiments.
