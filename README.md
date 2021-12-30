Geranium Core integration/staging tree
=====================================




Further information about Geranium Core is available in the [doc folder](/doc).

What is Geranium?
----------------

Geranium is an Decentralized crypto Asset/Currency,  that enables instant payments to
anyone, anywhere in the world. Geranium uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Geranium Core is the name of open source
software which enables the use of this currency.

More info:
Algorithm           : SHA256  <br>
Max supply          : 100 crore <br>
Circulating Supply  : 25 cr (subsidy halving= 1 crore blocks) <br>
Block Reward        : 25 coins perblock <br>
Block time          : 24s to 25s <br>
Difficulty Retarget : 77 hrs <br>

Use at own Risk: In development! <br>
Created by Manomay Mane,
Enjoy


License
-------

Geranium Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built (see `doc/build-*.md` for instructions) and tested, but it is not guaranteed to be
completely stable. [Tags](https://github.com/geranium/geranium/tags) are created
regularly from release branches to indicate new official, stable release versions of Geranium Core.

The main branch is the first or Genesis branch.

The https://github.com/geranium-core/gui repository is used exclusively for the
development of the GUI. Its master branch is identical in all monotree
repositories. Release branches and tags do not exist, so please do not fork
that repository unless it is for development reasons.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).
Anyone can help to develop the project!

Testing
-------

Testing and code review is the bottleneck for development;. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The CI (Continuous Integration) systems make sure that every pull request is built for Windows, Linux, and macOS,
and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[Geranium Core's Transifex page](https://www.transifex.com/geranium/geranium/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
