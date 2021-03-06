# PixelAnalysis
<p>
Project started by Sven T. Bitters, 2016<br>
Contact: sven.bitters@gmail.com
</p>

## Introduction
PixelAnalysis is an image anlysis tool for the evaluation of pixel intensity in micrographs written in MATLAB. 

The primary objective of PixelAnalysis is to aid researchers with the evaluation of fluorescence distribution across a cell in a micrograph. A possible usage scenario would be an experiment where a membrane-bound soluble protein of interest (e.g. tagged with a fluorescent protein) is expressed in a cell; then a competitor is added which displaces the protein from the membrane. With increasing competitor concentration more and more of the protein of interest will relocalize from the membrane to the cytoplasm which can be observed using a microscope - i.e. fluorescence of the membrane decreases, while general fluorescence of the cell increases. The general approach to quantifying the protein's displacement is measuring pixel intensity across many cells using a tool like ImageJ which returns a pixel intensity plot for each analysed cell. Further analysis of these plots then often proceeds by hand: the researcher first determines the pixel intensity of the cell membrane and then estimates the average pixel intensity of the cytoplasm (which may or may not be biased). Finally, the ratio between membrane and cytoplasmic pixel intensity is caluclated manually. All in all, this method is really laborious and consumes a lot of time - time that could have been spent on conducting another experiment.

Using PixelAnalysis this process is sped up heavily because after a micrograph has been imported to the software the user only has to place region of interest (ROI) lines across the relevant cells - the subsequent analysis steps are then automated as much as possible. PixelAnalysis determines membrane and cytoplasmic regions by itself, then measures mean pixel intensity, and in the end calculates the pixel intensity ratio between membrane and cytoplasm. Once all measurements are done, CellAnalysis returns a text file containing a list with membrane and cytoplasmic pixel intensity and their ratio of all selected cells together with the corresponding pixel intensity plots. 

## To Do
<ul>
  <li>Add some advanced options (e.g. user-defined decimal mark)</li>
  <li>Refine error handling</li>
  <li>Complete README</li>
<ul>
