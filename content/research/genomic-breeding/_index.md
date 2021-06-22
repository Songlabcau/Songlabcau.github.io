+++
# A Demo section created with the Blank widget.
# Any elements can be added in the body: https://wowchemy.com/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "blank"  # See https://wowchemy.com/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
# weight = 200  # Order that this section will appear.

title = "Genomic Breeding"
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

#### Genomic selection-assisted breeding mode

   Compared to molecular marker-assisted breeding (MAB), genomic selection (GS) is a new frontier that uses large numbers of SNP markers to predict breeding values to select candidate lines for hybridization. This process involves building a training population with known genotypes and phenotypes to construct GS model and derive the most optimal parameters for the model. Then, for a candidate population, using the genotype as input to predict the trait as output. This method can predict the simulated traits from all possible combination of parental lines in the test population, and then help to select parental lines for actual breeding. We are currently working in rice and maize to improve the GS model, by dissecting effective markers into additive, dominant, over-dominant, and epistatic classes, with quantitative evaluation of marker effects. When training the GS models, we utilize different methods including GBLUP, rrBLUP, Bayesian, and modern machine learning approach such as neural network, deep learning, SVM, RF, decision tree.

   {{< figure src="Genomic_Breeding.png" width="100%" >}}
