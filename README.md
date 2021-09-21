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

The mojchart colour palettes aim to be accessible to those with the most
common forms of colour blindness, and should also be discernable in
greyscale. The standard palettes in this package have been designed to
meet WCAG 2.0 accessibility guidance.

Four of the created palettes (`main.palette`, `electric.brights`,
`just.beachy` and `cycling.hills`) contain four colours each, and meet
WCAG 2.0 AAA guidance. All colours have a contrast ratio of at least
4.5:1 to the bars adjacent to them, and alternate light and dark shades
to further increase contrast. This is the highest standard of
accessibility and should be used when possible.

Two of the created palettes (`mountain.train` and `clear.skies`) contain
6 colours each, and meet WCAG 2.0 AA guidance. All colours have a
contrast ration of at least 3:1 to the bars adjacent to them, and
alternate light and dark shades to further increase contrast. This is
the minimum standard of accessibility required for publication and use
should be limited to times when a larger palette is required.

It is also possible to generate gradient palettes using this package,
with colours based on the DfT corporate theme. While these palettes can
be generated with any number of shades, there is no guarantee that the
contrast between these colours is sufficient to meet accessibility
standards. These palettes should only be used in very limited
circumstances where colour is not the only means of distinguishing
different groupings and none of the standard palettes are suitable.

For line charts, it may be possible that lines with reduced contrast are
next to each other. As a result, and in line with GSS recommendation,
line charts should be labelled directly where possible rather than using
a legend.
