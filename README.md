# fair-imaging-epfl

## Goals:

Detect astronomical sources using different tools and possibly interdisciplinary tools as well.
Compare the results with existing and established tools or catalogues, e.g. [DESI Legacy Survey](https://www.legacysurvey.org/) (that uses [tractor](https://github.com/dstndstn/tractor)).




## Data access:

A) IVOA standard [galaxy tool](https://usegalaxy.eu/root?tool_id=toolshed.g2.bx.psu.edu/repos/astroteam/astronomical_archives/astronomical_archives/0.10.0): 
  
  example of [workflow for EUCLID](https://usegalaxy.eu/u/avariu/w/query-euclid)
   
  
B) [DESI mmoda](https://gitlab.renkulab.io/astronomy/mmoda/desi-legacy-survey) / [galaxy tool](https://galaxy.odahub.fr/root?tool_id=toolshed.g2.bx.psu.edu/repos/astroteam/desi_legacy_survey_astro_tool/desi_legacy_survey_astro_tool/0.0.1+galaxy0)

C) [Euclid Image](https://euclid.caltech.edu/image/euclid20250319d-euclid-deep-field-south-70x-zoom)

D) [Euclid astroquery](https://astroquery.readthedocs.io/en/latest/esa/euclid/euclid.html#cutout-search)


## Methods:
A) From Mallory Wittwer  (Mail: 29.04.2025):
  1) [SEP](https://sep.readthedocs.io/en/stable/tutorial.html)
  3) Suggestions: [photutils, star finder algorithm](https://photutils.readthedocs.io/en/stable/user_guide/index.html),

B) [Nuclei Segmentation Boundary Model](https://bioimage.io/#/?id=10.5281%2Fzenodo.5764892)

## Progress:
A) Andrei:
  stored in [issue1](https://github.com/FAIR-imaging/OSCARS-FIESTA/issues/23#issuecomment-2804841724) and [issue2](https://github.com/FAIR-imaging/OSCARS-FIESTA/issues/1#issuecomment-2829873631)

  Summary:
  I used as input a single band out of the three that make this [Euclid Image](https://euclid.caltech.edu/image/euclid20250319d-euclid-deep-field-south-70x-zoom) and obtained this [output](./Galaxy13-Overlay-images-on-data-12-and-data-2-output_png.png)

  Based on this [tutorial](https://training.galaxyproject.org/training-material/topics/imaging/tutorials/process-image-bioimageio/tutorial.html):
  
  
  I have used nuclei-segmentation-boundarymodel in the galaxy workflow on an image pictured by EUCLID to obtain the attached figure. The only parameters I have changed are the size of the picture to 3840,2160,1,1. (this was not 100% obvious, but in the end I understood how it works).
  
  I would say the workflow provides some interesting results. However:
  1) it does not find all galaxies
  2) it provides structures that contain multiple galaxies ( this could be a positive aspect as well, but needs to be studied more)

  Questions:
  1) Are there some other parameters that could be interesting to change and see the effect on the final result?
  2) is there some other output of this workflow that quantifies the positions (and maybe the shape) of the structures so that I could compare this result with other methods?

B) Mallory:

[SEP Output image](mallory_sep_output.png)
  

## Suggestions
[Voronoi Segmentation for different scientific disciplines](https://github.com/galaxyproject/training-material/pull/5508#issuecomment-2830306324)

