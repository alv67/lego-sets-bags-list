# Various PYTHON codes

In this folder you can find different Python applications used to extract infromation
from the [Briklink Studio](https://www.bricklink.com/v3/studio/download.page) artefacts.

Here are same Jupyter projects :

## lego-parts-csv2md (Jupyter notebook)

Starting from a _Studio_ CSV exported project and extract parts, and create a _Markdown_ code
that can be copied into your document.
This create a single table with all the parts, adding link to _Bricklink_ page and using image
from the same _Bricklink_ page.

## lego-parts-io2md (Jupyter notebook)

This is a more articulated notebook that add more features:

- open the Studio project (non need to export to CSV)
- slits the part list depending on the _submodels_ of the project
- deep search for parts on the _Bricklink_ site
- automatic search for alternative parts that are different from Bricklink and LDraw
- create and uses a `parts-alternative.json`file to keep track of alternative parts
- Do not use the _Bricklink_ API (as need for authorized user) but uses the public HTML pages to get infos
- caches all the requests to _Bricklink_ site in order to reduce requests to the site

Also this notebook create a _Markdown_ code to be used in your project
