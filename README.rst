**NOTE:** Since July 2023, `obs-studio` uses an updated build system on Windows that automates most steps required in old build systems. Build instructions for the legacy build system for OBS Studio 28.0 to 29.1 are retained at [Legacy Build Instructions For Windows](https://github.com/obsproject/obs-studio/wiki/Legacy-Build-Instructions-For-Windows/).

## Prerequisites
* Windows 10 1909+ (or Windows 11)
* Visual Studio 2022 (at least Community Edition)
  * Windows 10 SDK (minimum 10.0.20348.0)
  * C++ ATL for latest v143 build tools (x86 & x64)
* Git for Windows
* CMake 3.24 or newer

## Configure Build Project

1. Clone the repository including **submodules**:

    `git clone --recursive https://github.com/obsproject/obs-studio.git`

2. Set current directory to `obs-studio`
3. Check available CMake presets: `cmake --list-presets`
4. Select the `windows-x64` preset: `cmake --preset windows-x64`
    - Available and supported architectures are: `x64`
      - x86 (32-bit) builds of obs-studio are no longer supported
    - Any other CMake variables can be provided as usual and can also override variables set by the preset if necessary

## Build obs-studio

1. Open the Visual Studio solution file in the generated build directory (`build_x64\obs-studio.sln`)
2. Select the build configuration that you want to build (Debug, MinSizeRel, Release, RelWithDebInfo)
3. Press `<Control>+<Shift>+<B>` to build the solution (Build -> Build Solution)
   1. Alternatively, press `<F5>` to build and run it (Debug -> Start Debugging)

OBS Studio <https://obsproject.com>
===================================

.. image:: https://github.com/obsproject/obs-studio/actions/workflows/push.yaml/badge.svg?branch=master
   :alt: OBS Studio Build Status - GitHub Actions
   :target: https://github.com/obsproject/obs-studio/actions/workflows/push.yaml?query=branch%3Amaster

.. image:: https://badges.crowdin.net/obs-studio/localized.svg
   :alt: OBS Studio Translation Project Progress
   :target: https://crowdin.com/project/obs-studio

.. image:: https://img.shields.io/discord/348973006581923840.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2
   :alt: OBS Studio Discord Server
   :target: https://obsproject.com/discord

What is OBS Studio?
-------------------

OBS Studio is software designed for capturing, compositing, encoding,
recording, and streaming video content, efficiently.

It's distributed under the GNU General Public License v2 (or any later
version) - see the accompanying COPYING file for more details.

Quick Links
-----------

- Website: https://obsproject.com

- Help/Documentation/Guides: https://github.com/obsproject/obs-studio/wiki

- Forums: https://obsproject.com/forum/

- Build Instructions: https://github.com/obsproject/obs-studio/wiki/Install-Instructions

- Developer/API Documentation: https://obsproject.com/docs

- Donating/backing/sponsoring: https://obsproject.com/contribute

- Bug Tracker: https://github.com/obsproject/obs-studio/issues

Contributing
------------

- If you would like to help fund or sponsor the project, you can do so
  via `Patreon <https://www.patreon.com/obsproject>`_, `OpenCollective
  <https://opencollective.com/obsproject>`_, or `PayPal
  <https://www.paypal.me/obsproject>`_.  See our `contribute page
  <https://obsproject.com/contribute>`_ for more information.

- If you wish to contribute code to the project, please make sure to
  read the coding and commit guidelines:
  https://github.com/obsproject/obs-studio/blob/master/CONTRIBUTING.rst

- Developer/API documentation can be found here:
  https://obsproject.com/docs

- If you wish to contribute translations, do not submit pull requests.
  Instead, please use Crowdin.  For more information read this page:
  https://obsproject.com/wiki/How-To-Contribute-Translations-For-OBS

- Other ways to contribute are by helping people out with support on
  our forums or in our community chat.  Please limit support to topics
  you fully understand -- bad advice is worse than no advice.  When it
  comes to something that you don't fully know or understand, please
  defer to the official help or official channels.
