pyIQM
=========

.. warning::
 This software is built on Python 2, and may or may not be converted to Python 3. It is largely a personal project and no support is provided, so please use at your own risk.


pyIQM is a library primarily for the purpose of convenience of the Broholm group at JHU for neutron scattering data analysis an materials characterization. It borrows a great deal from other useful libaries which are listed as dependences. The following classes are available.

    * SQW
        * Generically stores calculated or measured neutron data
        * Wrapper with convenient methods specifically powder data
        * Convenient correction functions that are often used like background subtraction.
        * 
        * 
    * Instrument
        * Borrowing heavily from neutronpy, can calculate resolution for various instrument settings.
        * Generically used to define neutron instrumentation.
    * Material
        * Initializes from a cif or can be built from space group symmetries and wyckoff positions
        * Contains all aspects of material relevant to neutron scattering
        * Magnetic form factor calculation
        * Normalization calculations
        * Can be combined with SQW or PPMS for modeling of materials
        * Methods for spinW, band structure, basic DFT
    * PPMS
        * Class for importing, plotting, and analyzing PPMS data with the following subgroups:
          * Heat Capacity
          * VSM / magnetization
          * AC Susceptibility
    * Data Handling
        * Fitting Functions
        * Generic helper functions like binning
        * Generic functions to plot arbitrary arrays
