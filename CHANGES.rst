===========
 Changelog
===========

1.2.1 (unreleased)
==================

- Nothing changed yet.


1.2.0 (2021-04-13)
==================

- Fixed XSS vulnerability on rating action
  [keul, cekk]

- Add support for Python 3.

- Add support for PyPy.

- Remove support for Python 2.6.

- Add support for zope.component 5.


1.1 (2013-09-20)
================

* Update to support Zope 2.13 and Plone 4.0 through 4.3 and clear up
  dependencies.


1.0-final (2011-08-21)
======================

* Template markup fixes for chameleon compatibility.

* Added Basque and Catalan translations.

1.0-rc3 (2011-05-12)
====================

* Optimize for average/count calculations with large numbers of
  ratings.  Improve performance of most recent rating lookup.

* Fixes for Plone 4.1

1.0-rc2 (2010-11-28)
====================

* Don't use a CSS id in view only rating view so that listings with
  ratings can still have valid html.


1.0-rc1 (2010-08-31)
====================

* Add support for view only rating views.

* Remove _v attribute caching.

* Plone 4 / Zope 2.12 compatibility (still works on Plone 3.3.4 / Zope 2.10.11):
    * permissions.py: Don't depend on Products.__ac_permissions__
    * Import ApplicationDefaultPermissions from AccessControl.Permission
    * Fix tests:
        * traverser.py, README.txt: SampleContainer class may come
          from zope.* and zope.app.*
        * utils.py: Date may or may not be followed by semicolon
    * browser/basic.py: add publishTraverse method to BasicEditorialRatingView,
      to prevent faulty traversal.
    * events.py and interfaces.py: Subclass IObjectRatedEvent from IObjectEvent
      (instead of from IObjectModifiedEvent) to prevent permissions errors.

* Added this file

0.2 (2009-05-11)
================
