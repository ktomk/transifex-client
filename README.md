Transifex Command-Line Tool
===========================
[![image](https://circleci.com/gh/transifex/transifex-client/tree/master.svg?style=shield&circle-token=33aafd984726261eff1b73278a0cf761382c478a)](https://circleci.com/gh/transifex/transifex-client/tree/master)
[![image](https://ci.appveyor.com/api/projects/status/github/transifex/transifex-client?branch=master&svg=true)](https://ci.appveyor.com/project/transifex/transifex-client/branch/master)
[![codecov](https://codecov.io/gh/transifex/transifex-client/branch/master/graph/badge.svg)](https://codecov.io/gh/transifex/transifex-client)
[![PyPI version](https://badge.fury.io/py/transifex-client.svg)](https://badge.fury.io/py/transifex-client)

> _⚠️ A new client, compatible with the [new API](https://transifex.github.io/openapi/), is under development. Check out the Alpha version [here](https://github.com/transifex/cli)._

## Getting started
Whether you have experience with the command line or not, [this interactive tutorial](https://www.transifex.com/learn/txclient/) is intended for everyone who wishes to learn how the Transifex client works. There is no need to download anything - Just click on the link provided above, and follow the instructions.

For more information about TX client, please visit our [documentation guide here](https://docs.transifex.com/client/introduction).

Description
---
The Transifex Command-line Tool enables you to manage your translations within a project without the need of an elaborate UI system.

You can use the command line tool to create new resources, map locale files to translations, and synchronize your Transifex project with your local repository. Translators and localization managers can use it to handle large volumes of translation files.  The Transifex Command-line Tool can help to enable continuous integration workflows and can be run from CI servers like Jenkins and Bamboo.

[Click  here](http://docs.transifex.com/client/) for complete documentation on the Transifex Command-line Tool via our documentation site.

Installation
------------

You can install the latest version of transifex-client running `pip install transifex-client` or `easy_install transifex-client`.

Build transifex-client for Windows
----------------------------------

1.  Download transifex-client sources via git or github archive.
    1.  `git clone https://github.com/transifex/transifex-client.git`
    2.  Download and unpack <https://github.com/transifex/transifex-client/archive/master.zip>

2.  Download and install [Python](https://www.python.org/downloads/windows/).

    At this step choose the right version of python (2.7, 3.5, 3.6 or 3.7) and x86 or x86-64 instruction set.

    Make sure pip marked for installation(default for latest installers).

3.  Install [PyInstaller](http://www.pyinstaller.org).

    Suppose that Python installed to `C:\\Program Files\\Python35-32`

    Make `python.exe` accessible via PATH environment variable or cd to directory containing python.exe.

        python -m pip install pyinstaller

    This command will install `PyInstaller` package and its dependencies.

4.  Build `transifex-client` distribution.

    Change directory to transifex-client folder and run command:

        python -m PyInstaller contrib/tx.spec
        # or
        pyinstaller contrib/tx.spec

5.  `tx.exe`

    `dist/tx.exe` will be created as the result of build process.


Getting Help
---
You can always get additional help via [GitHub issues](https://github.com/transifex/transifex-client/issues) or [Transifex support](https://www.transifex.com/contact/)

License
---
Transifex Client is primarily distributed under the terms of the GPL License (Version 2.0).

See [LICENSE](https://github.com/transifex/transifex-client/blob/master/LICENSE) for details.
