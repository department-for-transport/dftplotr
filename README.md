dftplotR
========

dftplotR is an R package to provide standardised charts formatting in
ggplot2. It includes theme functions which meet Government Statistical
Service (GSS) best practice guidance. It also includes colour palettes
based on DfT corporate branding which meet WCAG 2.0 accessibility
standards, and are distinguishable in greyscale.

Installation
------------

You can install dftplotR with:

    install.packages("devtools")
    devtools::install_github("departmentfortransport/dftplotr")

Overview
--------

The package contains the following functions:

`scale_colour_dft`: ggplot function which applies one of a range of DfT
palettes to a ggplot line chart (or other chart which groups by
**colour**)

`scale_fill_dft`: ggplot function which applies one of a range of DfT
palettes to a ggplot line chart (or other chart which groups by
**fill**)

`display_palette`: a visual output which shows all of the colours
contained in the selected DfT palette

`palette_picker_tool`: loads an interactive Shiny dashboard which allows
users to build their own custom palettes of up to 5 colours using the
DfT corporate colours.

Colour palettes
---------------

ggplot2 themes
--------------

Palette picker tool
-------------------

Accessibility
-------------
