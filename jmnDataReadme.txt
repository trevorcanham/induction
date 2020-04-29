%auto-ignore
Supplementary Data ReadMe  

Matching visual induction effects on screens of different size by regularizing a neural field model of color appearance
Trevor Canham, Javier Vazquez-Corral, Elise Mathieu, and Marcelo Bertalmío

The included .mat files contain a full array of observer responses for the chromatic and achromatic experiments reported in the paper, and sRGB arrays of the test patterns, with original and corrected versions (disparity between cinema and mobile conditions is compensated for in the test field based on observer responses). The experimental viewing environment was arranged such that 51 pixels on screen was equal to one visual degree for observers. There are two separate .mat files (which can be processed using Matlab or the free product octave) for the chromatic and achromatic experiments, which are named accordingly. An explanation of each file's contents is given below.

jmnDataChromatic.mat:
The data structure consists of three fields, each containing four cells. The cells correspond to color sets 1-4, shown in Figure 11 of the paper.

jmnData.resp - Observer responses encoded in L*a*b* - 4D array (2 x scaling factors [mobile,cinema], 3 x starting points [-10a*/b*, original value, +10a*b*], 3 x color channels [L*,a*,b*], 3-4 x observers)
jmnData.patchObs - The chromatic test patterns with test ring replaced by mean observer reported correction, encoded for sRGB display  - 3D array (801 rows x 1602 columns x 3 color channels)
jmnData.patchRef - The chromatic test patterns with test and comparison rings at their original, uncorrected values, encoded for sRGB display  - 3D array (801 rows x 1602 columns x 3 color channels)

jmnDataAchromatic.mat:
This dataset consists of three fields, each containing a single cell.

jmnData.resp - Observer response values encoded in sRGB - 4D array (5 x bar widths (visual degrees) [0.19,0.38,0.54,0.76,0.96], 3 x initial test bar values (cd/m^2) [4.0,8.1,22], 2 x pattern sides [white surround, black surround], 10 x observers)
jmnData.patchObs - The achromatic test patterns with test bars replaced by mean observer reported correction, encoded for sRGB display  - 3D array (740 rows x 1160 columns x 3 color channels x 5 target bar widths)
jmnData.patchRef - The achromatic test patterns with test and comparison bars at their original, uncorrected values, encoded for sRGB display  - 3D array (740 rows x 1160 columns x 3 color channels x 5 target bar widths) 