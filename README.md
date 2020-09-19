LibFolder
=========

Store libraries for use in the Desktop Development Environment.


Introduction
------------

LibFolder provides a home for libraries which are to be used with the DDE but do not wish to be integrated into its directory strcuture.

When seen by the Filer, or when double-clicked, LibFolder scans the Libs folder within it for sub-folders containing an Obey file named SetVars. Any such Obey files which are found will be passed to `*Filer_Run`.

Double-clicking on !LibFolder will also open the Libs folder within it, to allow new libraries to be installed.


Building
--------

LibFolder consists of a collection of un-tokenised BASIC, which must be assembled using the [SFTools build environment](https://github.com/steve-fryatt). It will be necessary to have suitable Linux system with a working installation of the [GCCSDK](http://www.riscos.info/index.php/GCCSDK) to be able to make use of this.

With a suitable build environment set up, making LibFolder is a matter of running

	make

from the root folder of the project. This will build everything from source, and assemble a working !LibFolder application and its associated files within the build folder. If you have access to this folder from RISC OS (either via HostFS, LanManFS, NFS, Sunfish or similar), it will be possible to run it directly once built.

To clean out all of the build files, use

	make clean

To make a release version and package it into Zip files for distribution, use

	make release

This will clean the project and re-build it all, then create a distribution archive (no source), source archive and RiscPkg package in the folder within which the project folder is located. By default the output of `git describe` is used to version the build, but a specific version can be applied by setting the `VERSION` variable -- for example

	make release VERSION=1.23


Licence
-------

LibFolder is licensed under the EUPL, Version 1.2 only (the "Licence"); you may not use this work except in compliance with the Licence.

You may obtain a copy of the Licence at <http://joinup.ec.europa.eu/software/page/eupl>.

Unless required by applicable law or agreed to in writing, software distributed under the Licence is distributed on an "**as is**"; basis, **without warranties or conditions of any kind**, either express or implied.

See the Licence for the specific language governing permissions and limitations under the Licence.
=======

Guess words from the ImpressionSpell dictionary.


Introduction
------------

LibFolder is a desktop implementation of the traditional word-guessing game. At the start of their turn, the player is presented with a random word in which all the letters have been replaced by dashes. Attempts must be made to guess the letters: if a guess is correct then that letter is shown in all its locations, but if wrong a "life" is lost. If the whole word has been guessed before all the available lives have gone, the player has won.


Building
--------

LibFolder consists of a collection of un-tokenised BASIC, which must be assembled using the [SFTools build environment](https://github.com/steve-fryatt). It will be necessary to have suitable Linux system with a working installation of the [GCCSDK](http://www.riscos.info/index.php/GCCSDK) to be able to make use of this.

With a suitable build environment set up, making LibFolder is a matter of running

	make

from the root folder of the project. This will build everything from source, and assemble a working !LibFolder application and its associated files within the build folder. If you have access to this folder from RISC OS (either via HostFS, LanManFS, NFS, Sunfish or similar), it will be possible to run it directly once built.

To clean out all of the build files, use

	make clean

To make a release version and package it into Zip files for distribution, use

	make release

This will clean the project and re-build it all, then create a distribution archive (no source), source archive and RiscPkg package in the folder within which the project folder is located. By default the output of `git describe` is used to version the build, but a specific version can be applied by setting the `VERSION` variable -- for example

	make release VERSION=1.23


Licence
-------

LibFolder is licensed under the EUPL, Version 1.2 only (the "Licence"); you may not use this work except in compliance with the Licence.

You may obtain a copy of the Licence at <http://joinup.ec.europa.eu/software/page/eupl>.

Unless required by applicable law or agreed to in writing, software distributed under the Licence is distributed on an "**as is**"; basis, **without warranties or conditions of any kind**, either express or implied.

See the Licence for the specific language governing permissions and limitations under the Licence.