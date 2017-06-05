## A Set of Notes for the Topic: *Applied Spatial Econometrics*

This is a basic guide to both the resources required and the required reading list for MSc Dissertation Topic number 103. While not exhaustive by any means, it provides a guide to the most useful tools and practices. To be clear, your objective should be to i.) either design an application of a spatial econometric model in some specific context which interests you, and then comment on how the results vary across choices of spatial weighting matrix, or ii.) use an existing dataset ([such as the Boston dataset augmented by Pace and Gilley (1997)](https://artax.karlin.mff.cuni.cz/r-help/library/spdep/html/boston.html)) and design a significant way to systematically evaluate the effect of spatial weighting matrix specification.

### Spatial Econometrics Textbooks

There are a number of books written by leading spatial econometricians. My favourite is the one by James LeSage and Robert Kelley Pace - [Introduction to Spatial Econometrics](https://www.amazon.co.uk/Introduction-Spatial-Econometrics-Statistics-Monographs/dp/142006424X/). Another is by J Paul Elhorst - [Spatial Econometrics: From Cross-Sectional Data to Spatial Panels](https://www.amazon.co.uk/Spatial-Econometrics-Cross-Sectional-SpringerBriefs-Regional/dp/3642403395). Another example is the forthcoming book by Harry Kelejian and Gianfranco Piras - [Spatial Econometrics](https://www.amazon.co.uk/Spatial-Econometrics-Harry-Kelejian/dp/0128133872/). However, there are surely many more and there are also a number of **free** online resources associated with specific software languages (see below).

### Software

You have three main options when it comes to statistical software for spatial econometric estimation. The first is the wonderful Spatial Econometrics Toolbox in MATLAB which is maintained by James LeSage. This is very well documented in [this](http://www.rri.wvu.edu/webbook/lesage/spatial/wbook.pdf) textbook. The second is the PySAL library, which is described in the documentation [here](http://pysal.readthedocs.io/en/latest/). The final choice is the R statistical programming language, to which a great guide written by Ignacio Sarmiento-Barbieri at the University of Illinois can be found [here](http://www.econ.uiuc.edu/~lab/workshop/Spatial_in_R.html). There is also a textbook specifically written for Spatial Econometrics in R by [Giuseppe Arbia](https://www.amazon.co.uk/Primer-Spatial-Econometrics-Applications-Palgrave/dp/1137428163/).

### The Application/Data

There are an absolutely enormous number of applications of various spatial econometric models all across the econometric literature. These include those within the fields of Trade, Environmental, Real Estate and Development economics. You have complete jurisdiction over what application you choose to utilize, although if you want to focus on a unique application, you will have to be responsible for putting together your own dataset and constructing your own spatial weighting matrices (approach i.) above). If you wanted to take an approach which examined spatial weighting matrix variation in some specific way, you can use one of the many 'off the shelf' datasets which already include geocoded co-ordinates (approach ii.) from above). Examples include the Boston dataset mentioned above, one of the examples which come packaged with James LeSages MATLAB toolbox, or the San Francisco housing dataset which comes with Adlers [textbook on R](https://www.amazon.co.uk/R-Nutshell-OReilly-Joseph-Adler/dp/144931208X).

### Spatial Weighting Literature

A significant part of the project is to examine variation over spatial weighting matrix space. This means that you should estimate various models and consider how your results vary (and whether they should). The seminal topic in this field is LeSage and Pace (2014) - [The Biggest Myth in Spatial Econometrics](http://www.mdpi.com/2225-1146/2/4/217). Of specific relevance is the 'boosting' method discussed by Kostov (2010) - [Model boosting for spatial weighting matrix selection in spatial lag models](http://journals.sagepub.com/doi/abs/10.1068/b35137). My own paper - [A Grid Based Approach to Spatial Weighting Matrix Specification](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2975838) might prove useful, and some associated code (which examines the Boston dataset) is available [here](https://github.com/crahal/SpatialGrid) on this Github also. You can estimate any type of model with any type of weighting matrix parameterization as you wish.