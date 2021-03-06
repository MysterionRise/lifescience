#################
Indigo 1.3.0 beta
#################

*31 Dec 2016*

*******
Summary
*******


**New features and improvements**:

* Lucene/SOLR cartdridge was added. See `documentation <https://github.com/epam/Indigo/blob/master/bingo/lucene/README.md>`__
* Name to structure prototype method was added. See :ref:`details <indigo-1.3.0b-name-to-structure>`
* Updated set of rules for CIP descriptors calculations
* Updated functionality for standardize method (option ``standardize-fix-direction-wedge-bonds`` ) for redirection stereo bonds out of cycle if it is possible. `fixed <https://github.com/epam/indigo/issues/49>`__ 
* Rendering sgroups `fixed <https://github.com/epam/indigo/issues/8>`__ 
* Depict version and inchi parameters `fixed <https://github.com/epam/indigo/issues/18>`__ 
* Charged pseudos rendering `fixed <https://github.com/epam/indigo/issues/41>`__ 
* Added support of saving reactions in CDXML format `fixed <https://github.com/epam/indigo/issues/52>`__ 
* OS X 10.11 support was added
* Keeping properties for reaction monomers was `fixed <https://github.com/epam/indigo/issues/53>`__ 
* clean2d() function for "small" layout changes was implemented
* New elements up to ``Uuo`` were added
* New method ``massComposition`` for elements mass calculation was added
* Added Sgroups (GEN, MUL, SRU, SUP types) support into CML loader/saver
* Dearomatization for R-Groups was `added <https://github.com/epam/indigo/issues/61>`__ 
* Fixed issue in Molfile loader for templates loading
* Modified encode/decode from ASCII to UTF-8 for support non-Latin characters in Indigo python output
* Added support Rgroup attachment points with query features combination
* Reaction Gross formula and mass were added
* Atom to atom mapping algorithm improvement (multiple matching possibility)
* Exception handling on macOS was `fixed <https://github.com/epam/indigo/issues/42>`__ 
* Added correct alias saving into V2000 molfile
* CTAB -> SCSR transformation algorithm was modified
* Reset settings method was `added <https://github.com/epam/indigo/issues/66>`__  for Indigo  
* New methods checkValence, checkQuery were added. 
* Other `features and fixes <https://github.com/epam/Indigo/milestone/3>`__ 


*******
Details
*******

.. _indigo-1.3.0b-name-to-structure:

=================
Name to Structure
=================

Currently, the following grammar elements are supported:

* Alkanes (-enes, -ynes) and its derivatives
* Locants expansion
* Cyclic alkanes (-enes, -ynes) and its derivatives
* Skeletal 'a' substitution
* Basic elements (up to number 100)
* Dictionary of trivial names (~150 names)
* Relaxed vs. strict IUPAC grammar (penta-1,3-diene vs. 1,3-pentadiene)

See some `examples <../../examples/name-to-structure.html>`__


