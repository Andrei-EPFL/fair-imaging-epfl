# fair-imaging-epfl

## Goals:

Detect astronomical sources using different tools and possibly interdisciplinary tools as well.
Compare the results with existing and established tools.


## Data access:

A) IVOA standard galaxy tool: https://usegalaxy.eu/root?tool_id=toolshed.g2.bx.psu.edu/repos/astroteam/astronomical_archives/astronomical_archives/0.10.0
  
  example of workflow for EUCLID
  https://usegalaxy.eu/u/avariu/w/query-euclid 
  
B) DESI mmoda/galaxy tool: https://gitlab.renkulab.io/astronomy/mmoda/desi-legacy-survey
https://galaxy.odahub.fr/root?tool_id=toolshed.g2.bx.psu.edu/repos/astroteam/desi_legacy_survey_astro_tool/desi_legacy_survey_astro_tool/0.0.1+galaxy0

C)https://euclid.caltech.edu/image/euclid20250319d-euclid-deep-field-south-70x-zoom

## Methods:
A) From Mallory Wittwer  (Mail: 29.04.2025):
  1) https://sep.readthedocs.io/en/stable/tutorial.html
  2) Suggestions: https://photutils.readthedocs.io/en/stable/user_guide/index.html ; https://photutils.readthedocs.io/en/stable/user_guide/detection.html

## Progress:
stored in https://github.com/FAIR-imaging/OSCARS-FIESTA/issues/23#issuecomment-2804841724 and https://github.com/FAIR-imaging/OSCARS-FIESTA/issues/1#issuecomment-2829873631

  Summary:
  I used as input a single band out of the three that make this picture: https://euclid.caltech.edu/image/euclid20250319d-euclid-deep-field-south-70x-zoom and obtained this output

  Based on this tutorial:
  https://training.galaxyproject.org/training-material/topics/imaging/tutorials/process-image-bioimageio/tutorial.html
  
  I have used nuclei-segmentation-boundarymodel in the galaxy workflow on an image pictured by EUCLID to obtain the attached figure. The only parameters I have changed are the size of the picture to 3840,2160,1,1. (this was not 100% obvious, but in the end I understood how it works).
  
  I would say the workflow provides some interesting results. However:
  
     1) it does not find all galaxies
     2) it provides structures that contain multiple galaxies ( this could be a positive aspect as well, but needs to be studied more)
  
  1)Are there some other parameters that could be interesting to change and see the effect on the final result?
  2) is there some other output of this workflow that quantifies the positions (and maybe the shape) of the structures so that I could compare this result with other methods?
  
  

## Suggestions
(Voronoi Segmentation for different scientific disciplines )
https://github.com/galaxyproject/training-material/pull/5508#issuecomment-2830306324
