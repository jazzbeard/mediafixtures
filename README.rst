=============
MediaFixtures
=============

The django fixtures support is nice, while not perfect, most of the time it
is really usefull. 

But it misses a function to add media files alongside the model-fixtures. If
you have a media-based site, it make the life of a developer much easier when
you can that at any time with a fresh system, that not only contains a example
database, but also the matching media files. 

Command: use_media_fixtures
===========================

With "use_media_fixtures" you can copy all media-files inside of the INSTALLED_APP
apps to your media directory in MEDIA_ROOT

It will also overwrite existing files, even in existing directories. It searches
all installed apps for a directory named "media" in the fixtures directory.

Example:
  myownapp/fixtures/media/

The fixtures directory in the project itself is ignored (for now)