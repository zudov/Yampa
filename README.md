[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ivanperez-keera&url=https://github.com/ivanperez-keera/Yampa&title=Yampa&language=&tags=github&category=software)

Domain-specific language embedded in Haskell for programming hybrid (mixed
discrete-time and continuous-time) systems. Yampa is based on the concepts of
Functional Reactive Programming (FRP) and is structured using arrow
combinators.

NOTE: A new version of Yampa is under the works. It's maintained in a separate
branch, and will be merged with master. If you are FRP savvy, please take a
look around and tell us whether there's anything you'd change.  The
documentation is available at:
http://ivanperez-keera.github.io/haddock/Yampa/FRP-Yampa.html

# Installation

```
$ cabal sandbox init         # Optional, but recommended
$ cabal update
$ cabal install Yampa
```

# Examples

There are many programs written in Yampa. See the following examples:

* Haskanoid: a game that uses SDL multimedia, wiimote and kinect.
  https://github.com/ivanperez-keera/haskanoid
  http://hackage.haskell.org/package/haskanoid
* Space invaders: a demonstration game used for a paper.
  https://hackage.haskell.org/package/SpaceInvaders
* Frag: a 3D first person shooting game.
  https://hackage.haskell.org/package/frag

A more comprehensive list can be obtained using the reverse dependency finder
(http://packdeps.haskellers.com/reverse/Yampa), but only programs uploaded to
hackage are listed.

# Backends

Yampa is backend agnostic, you can ultimately connect it to any backend you
want. Existing backends include:
* SDL
* OpenGL / GLUT
* WX (see wxHaskell)

# Use in production

* Keera Studios is using it for several Haskell games for Android.
  http://facebook.com/keerastudios

# Documentation and tutorials

The distribution of Yampa comes with subtantial haddock documentation, which you can
build using haddock or just [read online](https://hackage.haskell.org/package/Yampa).
To build a local copy, do:

```
$ cabal unpack Yampa ## Or git clone this-repo
$ cd Yampa-*
$ cabal init
$ cabal install --only-dependencies
$ cabal configure && cabal haddock --internal
```

Documentation is also available online: https://wiki.haskell.org/Yampa

# Papers and technical reports

For a list of Yampa-related papers, see:

* http://www.cs.nott.ac.uk/~nhn/papers.html

See also PhD technical report, chapter 3. http://www.cs.nott.ac.uk/~ixp/
which includes a review of FRP and outlines some existing issues.

# Help and collaboration

You can collaborate at least in three ways:

* File an issue (https://github.com/ivanperez-keera/Yampa/issues).
* Write documentation (send a link and/or a pull request).
* Research: we are constantly trying to improve Yampa. We'd be glad to have
  collaborators.  If you are working on this, please, let us know.

  (_Interactivity and FRP is the main topic of my (ongoing) PhD studies, so I'll
  keep working on this for quite some time._ -- Ivan Perez)

# Authors

* Henrik Nilsson
* Antony Courtney

## Maintainer

* Ivan Perez
