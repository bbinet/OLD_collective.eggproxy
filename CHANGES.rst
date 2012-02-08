Changelog
=========


0.6 (unreleased)
----------------

- Nothing changed yet.


0.5.1 (2009-10-19)
------------------

- Added svn url to README.  [reinout]


0.5 (2009-10-19)
----------------

- Release fixes (setup.cfg that resulted in a horrid "0.4dev-r1234" release).
  No functional changes.


0.4 (2009-10-19)
----------------

- Fix compatibility issue with Python 2.6 New python version disallow to use
  config.add_section('DEFAULT') (see : http://bugs.python.org/issue1781 and
  ConfigParser documentation).  Patch by Stephane Klein.

- Updated maintainer email address.  [reinout]


0.3.1 (2009-04-28)
------------------

- Fix for non-updating index pages despite ALWAYS_REFRESH setting. Cause:
  already downloaded urls were not re-processed.  [reinout]


0.3 (2009-03-16)
----------------

- Updated documentation for buildout change and always_refresh change.
  [reinout]

- Attempt ../etc/eggproxy.conf as config location to help buildout setups.
  [reinout]

- Added always_refresh (and timeout) option to always attempt a real pypi
  connection to ensure freshness.  [reinout]

- Added port option to configuration. [reinout]

- don't lowercase package names

- improve wsgi app

- add tests


0.2.0 (2008-09-22)
------------------

- initial version as collective.eggproxy. This package was formerly known as
  iw.eggproxy (https://ingeniweb.svn.sourceforge.net/svnroot/ingeniweb/iw.eggproxy)

- package index/download files: skip modules installed in local system (resulted
  in copying a directory instead of downloading a file)

- fixed Update script crashing with invalid/obsolete package name

- Overriden PackageIndex so that we get eggs distributions for all versions, all
  platforms

- fixed malformed tag in generated indexes

0.1.0 (2008-06-06)
------------------

- initial version created by IngeniSkel
