# User Guide

## Overview

A general overview of the motivation for, benefits and functionality of the toolbox, as implemented in
**ITVizion Visualization toolbox**, is provided in this section. A guide for browsing through and using each plot is presented below.

## Violin Plot


The Violin plot class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a violin plot, distribution plot and line plot of available signals.



<video width="560" height="340" controls>
  <source src="_static/Violin Plot.MOV" type="video/mp4">
</video>



Through the interface, the user has the ability to select multiple signals by holding the CTRL button and clicking or using the Shift button and keyboard arrows, or select all using the checkbox right below. 


<br>
<table border="0">
 <tr>
    <td><img alt="image" src="_static/violin_plot_ui.png"></td>
 </tr>
 <tr>
    <td>Figure 1. User Interface of the Violin plot add-on.</td>
 </tr>
</table>
<br>


Furthermore, the "Sampling Interval" field provides for an interval to sample the signals' data. The user can fill the field using a variety of options, from seconds, to days and months. Then, the start and end date of the data need to be selected.

Finally, the last two checkboxes provide for:
    - *Normalize data*: data of each signal are subtracted their mean and divided by their standard deviation in order to bring them to a scale that allows for plotting them together in the same figure.
    - *Plot Distribution*: histograms including their mean value are generated for each signal.

On the plot, the user can hover over the violin plot in order to access calculations such as the mean, standard deviation, kernel density estimation and other. The user will also be able to zoom in and out, hide signals, download the figures and more, using the buttons on the top right corner.

Lastly, a static line plot is generated for all the plots and shown at the bottom of the output.


## Interactive Pairplot


The Pairplot_interactive class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a pairplot of available signals and allows users to select signals, generate plots and colour by the desired string column. 



<video width="560" height="340" controls>
  <source src="_static/Interactive pair plot.MOV" type="video/mp4">
</video>



Through the interface, the user has the ability to select multiple signals by holding the CTRL button and clicking or using the Shift button and keyboard arrows, or select all using the checkbox right below. 

<br>
<table border="0">
 <tr>
    <td><img alt="image" src="_static/pair_plot_ui.png"></td>
 </tr>
 <tr>
    <td>Figure 2. User Interface of the Interactive Pairplot add-on.</td>
 </tr>
</table>
<br>


Furthermore, the "Sampling Interval" field provides for an interval to sample the signals' data. The user can fill the field using a variety of options, from seconds, to days and months. Then, the start and end date of the data need to be selected.

After clicking the plotting button, if lexical expressions/string values are present in the data from the different signals, the add-on recognizes them and provides for a selection box that would colour the plot by the different values of the selected signal.

<br>
<table border="0">
 <tr>
    <td><img alt="image" src="_static/pair_plot_colour_by.png"></td>
 </tr>
 <tr>
    <td>Figure 3. Colour by option for string values.</td>
 </tr>
</table>
<br>

On the plot, the user can hover over the violin plot in order to access the values at selected points. The user will also be able to zoom in and out, hide signals, download the figures and more, using the buttons on the top right corner.


## Static Pairplot


The Pairplot class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a static pairplot and line plot of available signals and allows users to select signals, generate plots and colour by the desired string column.



<video width="560" height="340" controls>
  <source src="_static/Pair Plot.mov" type="video/mp4">
</video>




Through the interface, the user has the ability to select multiple signals by holding the CTRL button and clicking or using the Shift button and keyboard arrows, or select all using the checkbox right below. 


<br>
<table border="0">
 <tr>
    <td><img alt="image" src="_static/static_pair_plot_ui.png"></td>
 </tr>
 <tr>
    <td>Figure 4. User Interface of the Static Pairplot add-on.</td>
 </tr>
</table>
<br>



Furthermore, the "Sampling Interval" field provides for an interval to sample the signals' data. The user can fill the field using a variety of options, from seconds, to days and months. Then, the start and end date of the data need to be selected.



After clicking the plotting button, if lexical expressions/string values are present in the data from the different signals, the add-on recognizes them and provides for a selection box that would colour the plot by the different values of the selected signal.

<br>
<table border="0">
 <tr>
    <td><img alt="image" src="_static/pair_plot_colour_by.png"></td>
 </tr>
 <tr>
    <td>Figure 5. Colour by option for string values.</td>
 </tr>
</table>
<br>

Lastly, a static line plot is generated for all the plots and shown at the bottom of the output.