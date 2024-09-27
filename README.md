# adcTs1


File Access: It opens a ROOT file named "ZDCAnalyzer_USC_uncovered.root" that contains data related to a Zero Degree Calorimeter (ZDC) analysis.

Tree Access: It retrieves a specific tree named "Events" from the "zdcanalyzer" directory within the ROOT file. This tree contains event-based data for the ZDC.

Branch Setup: The code connects two branches ("zdcdigi_adcTs1" and "zdcdigi_adcTs0") from the tree to two arrays (zdcdigi_tdcTs1[26] and zdcdigi_tdcTsO[26]), which hold timing data for the ZDC's Time-to-Digital Converter (TDC).

Histogram Creation: A histogram named hZDC is created to store and visualize the data from the zdcdigi_adcTs1 branch.

Event Loop: The code loops over all entries in the tree, retrieves each entry's data, and fills the histogram with the first value (zdcdigi_tdcTs1[0]) from the array zdcdigi_adcTs1.

Plotting: After processing the data, it creates a canvas and plots the histogram (with the color set to blue) showing the distribution of adcTs1 values.

Saving Plot: The resulting plot is saved as an image file (adcTs1.png) in a specified directory.

Clean-Up: It closes the ROOT file after processing is complete.

This code is used to analyze and visualize timing data from the ZDC by creating a histogram of adcTs1 values and saving the plot for further study.
