# Home Assistant Theme: Outline-Edge

The original purpose of the theme was to restore the look and feel of HomeAssistant after the changes implemented in the 2022.11.1 Update, where the UI was adapted more to the Google Metro UI with larger border-radius and a slight border around all the cards.

The theme does provide the "original" Theme, but as well some more options where I've added some variations of the card borders as well.
In Addition, HA implemented more state color options with the December Updates (2022.12.x).

The "HA default" Theme is trying to restore [most] of the Icon colors to the previous state colors, but it does not cover all of them!
Some entities will still have new colors when they are active.

The other variants will make more use of the new color schemas but is trying to reduce the amount of different colors by a lot.
Most active sensors will be green when active, some of them will be red when active... this depends on the device class and if HA does provide new state colors for this device class (which is not always the case).

![grafik](https://user-images.githubusercontent.com/26391061/211516166-90fb898f-6cb6-46d6-96d3-9ebb7e3c9935.png)

## Installation

Add the following code to your `configuration.yaml` file (restart required).

```yaml
frontend:
  ... # your configuration.
  themes: !include_dir_merge_named themes
  ... # your configuration.
```

### Manual Installation

Clone this repository in your existing (or create it) `themes/` folder.

```bash
cd themes/
git clone https://github.com/ChristophCaina/home-assistant-theme-outline-edge
```

## Changelog & Releases

This repository keeps a change log using [GitHub's releases][releases]
functionality.

Releases are based on [Semantic Versioning][semver], and use the format
of `MAJOR.MINOR.PATCH`. In a nutshell, the version will be incremented
based on the following:

- `MAJOR`: Incompatible or major changes.
- `MINOR`: Backwards-compatible new features and enhancements.
- `PATCH`: Backwards-compatible bugfixes and package updates.

## Contributing

This is an active open-source project. We are always open to people who want to
use the code or contribute to it.

We've set up a separate document for our
[contribution guidelines](CONTRIBUTING.md).

Thank you for being involved! :heart_eyes:

## Authors & contributors

The original setup of this repository is by [Franck Nijhof][frenck].

For a full list of all authors and contributors,
check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2021-2022 Franck Nijhof

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Todo:
add new state variables from 2022.12.07
