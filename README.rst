
Python GUI Implementation
========

This is an exploration of building local Python applications with GUI. This
instance is based on a Data Dependence article by Moir. This document is
entitled How to Build a GUI in Python 3.5 and found at
"http://www.datadependence.com/2016/04/how-to-build-gui-in-python-3/".

The code in this repository includes extensions and modification to the
original work to address additional functionality questions that I chose to
pursue and shortcomings in the published work.

A toy application is considered where the goal is to accept two numbers as input
and provide a sum in an answer field. The real purpose is more to explore the
interface elements and understand the overall implementation issues for the GUI.
The work is based on Python 3.5 and tkinter.


Features & Modifications
--------

- "ttk" elements used for added style value.
- Simple adder program demonstrates tkinter GUI development in Python3.
- Added shell commands at top allowing direct program execution.
- Changed __init__ function to conform with current tkinter docunentation.
- on_quit with root.destroy() vs. quit() because quit did not give a clean exit.
The program execution ended but the main window remained open but
non-functional. Ran into issues in getting root.destroy operating because of
argument requirements calling on_quit. Seems that self is passed unspecified.
- Added styled tkinter QUIT button. This was used to test when working out menu
issues.
- Included separation of root window and contained app in __main__.

Installation
------------

None. This program is intended for standalone use from command line or Idle.
Configured code file for execution with proper privilege.

Contribute
----------

- Issue Tracker: github.com/fpr3/python_GUI/issues
- Source Code: github.com/fpr3/python_GUI

Support
-------

Please make contact through github conserning and issues or observations.
Thanks.

License
-------

No licensing is currently associated with this project. The project currently
only exists for educational purposes and primarily implements code presented in
the online article identified above.
