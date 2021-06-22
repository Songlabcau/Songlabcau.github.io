+++
# A Demo section created with the Blank widget.
# Any elements can be added in the body: https://wowchemy.com/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "blank"  # See https://wowchemy.com/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
# weight = 200  # Order that this section will appear.

title = "Bioinformatics"
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

#### An intelligent marker-selection system for crop (rice, maize, wheat) genetic breeding

   Previous GWAS and resequencing analysis of crop germplasm has identified millions SNP markers that can be selected for breeding purposes. One of the projects in the lab is to collect all previous published GWAS datasets, and to perform a meta-GWAS analysis to define significant haplotype block, SNP marker and genes in association with important agronomic traits. Similar to the concept in precision medicine, the basic idea of this work is to build up the link at different levels of biological entities with a series of feature tags. When a user define a trait or a breeding goal, the system will be automatically searching the databases with feature tags and finally result in collecting a panel SNP markers that can be used for molecular breeding or calculation of breeding values.


   Behind the database, we are using a set of machine learning techniques to organize the data. For instance, association rule learning (ARL) methods to automatically infer the relationships between different entities; when extracting a desired trait for improvement, a Random Forest (RF) model will be used to compile the best set of markers. In addition, we are also integrating a series of tools that are frequently used for molecular breeding in the database, so that user can do a one-stop analysis for crop breeding.
   {{< figure src="Bioinformatics.png" width="100%" >}}
