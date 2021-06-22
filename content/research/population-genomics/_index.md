+++
# A Demo section created with the Blank widget.
# Any elements can be added in the body: https://wowchemy.com/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "blank"  # See https://wowchemy.com/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
# weight = 200  # Order that this section will appear.

title = "Population Genetics"
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

For genetic improvement of crop species, genome-wide association analysis (GWAS) is a rapid way to identify the genes contributing to the variation of important agronomic traits, and the behind principles are population genetics. Since the Wang Lab moved to CAU, we started to work on GWAS of crop germplasm with new methods and new idea. We are working on GWAS in maize, rice, wheat. In a long run, we will construct a database for trait-related genes, tag SNPs, QTLs, and use these sets of information to support crop breeding.

1. #### Wheat population

   We GWASed a collection of wheat core germplasm with detailed records of spike trait, using ILLUMINA RNA-Seq. With eQTL analysis, we identified a series of candidate genes that may contribute to the wheat spike development. We also provide transgenic evidence to prove the functions of the genes we identified.
   {{< figure src="Population_Genetics_1.png" width="100%" >}}

2. #### Rice population
   Rice, Oryza sativa L., is the staple food for half the world’s population. Based on a resequenced core collection of 3,000 rice accessions from 89 countries, we utilized a series of evolutionary analytical and population methods to determine the frequently selected regions, genes and markers during the domestication and genetic improvement process in rice. From this dataset, our ultimate goal is to construct a database that includes all kinds of trait-related genes, markers and regions to provide a scalable, dynamic environment for rice researcher to extract important genes for breeding purpose.
   {{< figure src="Population_Genetics_2.png" width="100%" >}}
