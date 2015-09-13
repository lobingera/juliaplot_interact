Julia has with Gtk.jl already a low-to-high level adaption to the Gtk toolkit.

Some functions that are needed or considered to be of value for interaction with a user doing plotting are 
* selection - two parts: highlighting (i.e. showing some different marker/color on plot) and GUI input to select (e.g. rubberbanding, selection by single mouse click etc.)
* zoom/pan - zoom: changeing the scaling factor between data and projected data, pan: translating the view
* info - get information about the data / datapoint with selection

Examples:

https://gist.github.com/lobingera/2e7a9e4f8579b82d9fe5
An example by lobingera on selection and zoom/pan. The gist works with recent master on Gtk.jl and Cairo.jl.

https://github.com/timholy/GtkUtilities.jl
Build on Gtk and the GtkCanvas which includes hooks for interaction on mouse pointer, mouse buttons, modifiers (keys: shift, alt, ctrl etc.) and the scroll-wheel (button4).
