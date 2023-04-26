# Introduction

**ITV-visual** is a Python module to visualize selected signals of a workbook in a variety of plots. The package offers a static and an interactive version of a pairplot, 
distribution plots, line plots and violin plots. After applying the necessary data transformations, the former plots are a practical and direct way of understanding the distribution of the data
per parameter and identifying their relationships. The module includes a user interface (UI) designed to interact with the Seeq server. Specifically, the UI can be installed as an Add-on Tool
in Seeq Workbench.


# Installation

The backend of **ITV-visual** requires **Python 3.7** or later.

## Dependencies

See `requirements.txt` file for a list of
dependencies and versions. Additionally, you will need to install the `seeq` module with the appropriate version that
matches your Seeq server. For more information on the `seeq` module see [seeq at pypi](https://pypi.org/project/seeq/)

## User Installation Requirements (Seeq Data Lab)

If you want to install **ITV-visual** as a Seeq Add-on Tool, you will need:

- Seeq Data Lab (>= R52.1.5, >=R53.0.2, or >=R54)
- `seeq` module whose version matches the Seeq server version
- Seeq administrator access
- Enable Add-on Tools in the Seeq server

## User Installation (Seeq Data Lab)

The latest build of the project can be found [here](https://pypi) as a wheel file. The
file is published as a courtesy to the user, and it does not imply any obligation for support from the publisher.

1. Create a **new** Seeq Data Lab project and open the **Terminal** window
2. Run `pip install ITV_visual`
3. Import and use preferred classes in your python scripts by providing only the workbook url

or use directly as an add-on through the preferred seeq workbook.


# User Guide

## Overview

A general overview of the motivation for, benefits and functionality of the toolbox, as implemented in
**ITVizion Visualization toolbox**, is provided in this section. A guide for browsing through and using each plot is presented below.

## Violin Plot


The Violin plot class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a violin plot, distribution plot and line plot of available signals.

<br>
<table border="0">
 <tr>
    <td><img alt="image" src="docs/_static/violin_plot_ui.png"></td>
 </tr>
 <tr>
    <td>Figure 1. User Interface of the Violin plot add-on.</td>
 </tr>
</table>
<br>

Through the interface, the user has the ability to select multiple signals by holding the CTRL button and clicking or using the Shift button and keyboard arrows, or select all using the checkbox right below. 

Furthermore, the "Sampling Interval" field provides for an interval to sample the signals' data. The user can fill the field using a variety of options, from seconds, to days and months. Then, the start and end date of the data need to be selected.

Finally, the last two checkboxes provide for:
    - *Normalize data*: data of each signal are subtracted their mean and divided by their standard deviation in order to bring them to a scale that allows for plotting them together in the same figure.
    - *Plot Distribution*: histograms including their mean value are generated for each signal.

On the plot, the user can hover over the violin plot in order to access calculations such as the mean, standard deviation, kernel density estimation and other. The user will also be able to zoom in and out, hide signals, download the figures and more, using the buttons on the top right corner.

Lastly, a static line plot is generated for all the plots and shown at the bottom of the output.


## Interactive Pairplot


The Pairplot_interactive class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a pairplot of available signals and allows users to select signals, generate plots and colour by the desired string column. 

<br>
<table border="0">
 <tr>
    <td><img alt="image" src="docs/_static/pair_plot_ui.png"></td>
 </tr>
 <tr>
    <td>Figure 2. User Interface of the Interactive Pairplot add-on.</td>
 </tr>
</table>
<br>

Through the interface, the user has the ability to select multiple signals by holding the CTRL button and clicking or using the Shift button and keyboard arrows, or select all using the checkbox right below. 

Furthermore, the "Sampling Interval" field provides for an interval to sample the signals' data. The user can fill the field using a variety of options, from seconds, to days and months. Then, the start and end date of the data need to be selected.

After clicking the plotting button, if lexical expressions/string values are present in the data from the different signals, the add-on recognizes them and provides for a selection box that would colour the plot by the different values of the selected signal.

<br>
<table border="0">
 <tr>
    <td><img alt="image" src="docs/_static/pair_plot_colour_by.png"></td>
 </tr>
 <tr>
    <td>Figure 3. Colour by option for string values.</td>
 </tr>
</table>
<br>

On the plot, the user can hover over the violin plot in order to access the values at selected points. The user will also be able to zoom in and out, hide signals, download the figures and more, using the buttons on the top right corner.


## Static Pairplot


The Pairplot class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a static pairplot and line plot of available signals and allows users to select signals, generate plots and colour by the desired string column.


<br>
<table border="0">
 <tr>
    <td><img alt="image" src="docs/_static/static_pair_plot_ui.png"></td>
 </tr>
 <tr>
    <td>Figure 4. User Interface of the Static Pairplot add-on.</td>
 </tr>
</table>
<br>



Through the interface, the user has the ability to select multiple signals by holding the CTRL button and clicking or using the Shift button and keyboard arrows, or select all using the checkbox right below. 

Furthermore, the "Sampling Interval" field provides for an interval to sample the signals' data. The user can fill the field using a variety of options, from seconds, to days and months. Then, the start and end date of the data need to be selected.



After clicking the plotting button, if lexical expressions/string values are present in the data from the different signals, the add-on recognizes them and provides for a selection box that would colour the plot by the different values of the selected signal.

<br>
<table border="0">
 <tr>
    <td><img alt="image" src="docs/_static/pair_plot_colour_by.png"></td>
 </tr>
 <tr>
    <td>Figure 5. Colour by option for string values.</td>
 </tr>
</table>
<br>

Lastly, a static line plot is generated for all the plots and shown at the bottom of the output.

# Documentation

### Violin Plot


The Violinplot class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a violin plot, distribution plot and line plot of available signals.

Through the interface, the user has the ability to select multiple signals (holding the CTRL button and clicking or using the Shift button and keyboard arrows) to visualize and either generate the violin plots in separate figures or plot on the same figure by clicking on the option to normalize the data. Violin plots include certain calculations such as the mean, standard deviation, kernel density estimation and other. The user will also be able to zoom in and out, hide signals, download the figures and more.


### Interactive Pairplot


The Pairplot_interactive class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a pairplot of available signals and allows users to select signals, generate plots and colour by the desired string column. 

Through the interface, the user has the ability to select multiple signals (holding the CTRL button and clicking or using the Shift button and keyboard arrows) to visualize. The user will also be able to zoom in and out, hide signals, download the figures and more.



### Static Pairplot


The Pairplot class initializes an object that builds a GUI for an analysis worksheet provided through its URL. The GUI displays a static pairplot and line plot of available signals and allows users to select signals, generate plots and colour by the desired string column. Through the interface, the user has the ability to select multiple signals (holding the CTRL button and clicking or using the Shift button and keyboard arrows) to visualize.
