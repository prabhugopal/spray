.. _FileAndResourceDirectives:

FileAndResourceDirectives
=========================

Like the :ref:`RouteDirectives` the ``FileAndResourceDirectives`` are somewhat special in spray's routing DSL.
Contrary to all other directives they do not produce instances of type ``Directive[L <: HList]`` but rather "plain"
routes of type ``Route``.
The reason is that they are not meant for wrapping an inner route (like most other directives, as intermediate-level
elements of a route structure, do) but rather form the actual route structure **leaves**.

So in most cases the inner-most element of a route structure branch is one of the :ref:`RouteDirectives` or
``FileAndResourceDirectives``.

.. toctree::
   :maxdepth: 1

   getFromBrowseableDirectory
   getFromBrowseableDirectories
   getFromDirectory
   getFromFile
   getFromResource
   getFromResourceDirectory
   listDirectoryContents
   respondWithLastModifiedHeader
