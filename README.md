INTRODUCTION
============

SceneGlyph is a simple C++11 library for arranging nodes of text hierarchically
in 2D space, very similar to how traditional "scene graph" libraries arrange
and transform geometric objects. It is not bound to a particular rasterization
or rendering backend, though Cairo and OpenGLES2 were the original targets,
and the API may have lingered towards most easily facilitating those libraries.

API OVERVIEW
============

The following is a list of all of the main objects in the Sceneglyph library.

- Font: A Font holds all the data necessary to convert a unicode character into a 2D glyph.
- FontMap: A FontMap is a dictionary and resource manager for Font objects.
- Node: A Node is the basic unit of styled text in a Scene.
- Scene: A Scene contains a grouping of Node objects, and manages the physical layout of the
  text.
- State: A State object contains all the applicable styling data for a particular Node.

BUILD DEPENDENCIES
==================

- Harfbuzz
- libicu

