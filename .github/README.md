# CSS Navigation Menu
[heading__top]:
  #css-navigation-menu
  "&#x2B06; Pure CSS and HTML navigation menu example"


Pure CSS and HTML navigation menu example


## [![Byte size of CSS Navigation Menu][badge__gh_pages__css_navigation_menu__source_code]][css_navigation_menu__gh_pages__source_code] [![Open Issues][badge__issues__css_navigation_menu]][issues__css_navigation_menu] [![Open Pull Requests][badge__pull_requests__css_navigation_menu]][pull_requests__css_navigation_menu] [![Latest commits][badge__commits__css_navigation_menu__gh_pages]][commits__css_navigation_menu__gh_pages] [![css-navigation-menu Demos][badge__gh_pages__css_navigation_menu]][gh_pages__css_navigation_menu]


---


- [:arrow_up: Top of Document][heading__top]

- [:building_construction: Requirements][heading__requirements]

- [:zap: Quick Start][heading__quick_start]

- [&#x1F9F0; Usage][heading__usage]

- [&#x1F5D2; Notes][heading__notes]
  - [`index.html`][heading__indexhtml]
  - [`assets/css/style.css`][heading__assetscssstylecss]

- [:chart_with_upwards_trend: Contributing][heading__contributing]
  - [:trident: Forking][heading__forking]
  - [:currency_exchange: Sponsor][heading__sponsor]

- [:card_index: Attribution][heading__attribution]

- [:balance_scale: Licensing][heading__license]


---



## Requirements
[heading__requirements]:
  #requirements
  "&#x1F3D7; Prerequisites and/or dependencies that this project needs to function properly"


A web-browser is required to interact with rendered `index.html` file. For local testing some form of web-server may be necessary, eg...


```bash
cd ~/git/hub/web-dev-examples/css-navigation-menu

python3 -m http.server --bind 127.0.0.1 8080
```


... Alternatively this repository may be deployed and served via GitHub Pages.


______


## Quick Start
[heading__quick_start]:
  #quick-start
  "&#9889; Perhaps as easy as one, 2.0,..."


Clone this project...


**Linux/MacOS**


```Bash
mkdir -vp ~/git/hub/web-dev-examples

cd ~/git/hub/web-dev-examples

git clone git@github.com:web-dev-examples/css-navigation-menu.git
```


**Windows**


```Batch
set _organization_directory="%HOMEDRIVE%%HOMEPATH%\git\hub\web-dev-examples"

if not exists %_organization_directory (
  md %_organization_directory
)

CD /D %_organization_directory

git clone git@github.com:web-dev-examples/css-navigation-menu.git
```


______


## Usage
[heading__usage]:
  #usage
  "&#x1F9F0; How to utilize this repository"


Use a mouse or <kbd>Tab</kbd> key to focus the _`Menu`_ label and either click, or use <kbd>Enter</kbd> or <kbd>Space</kbd> keys, to open the menu.


Once open use the mouse, or <kbd>Tab</kbd> key, to select a link to navigate to.


Clicking out of the menu bounds will automatically close the menu.


Prefix the URL with `view-source:` to explore the served source code, eg...


```
view-source:https://web-dev-examples.github.io/css-navigation-menu/index.html
```


______


## Notes
[heading__notes]:
  #notes
  "&#x1F5D2; Information about source code"


> Information about source code


Current limitations of using only HTML and CSS;


- the <kbd>Esc</kbd> key without JavaScript will **not** close opened menu(s)

- the <kbd>Tab</kbd> key may focus elements other than those listed within top-most menu

- the menu width, and label, adjusts to widths of inner content


---


### `index.html`
[heading__indexhtml]: #indexhtml



> [`index.html`][branch__current__index_html] contains HTML5 elements that define page structure, and inline CSS3 is leveraged to provide core menu functionality.


The `lebel` and `input` checkbox elements are _tied_ to one-another via `id` and `for` attributes, eg...


```html
<input id="session_state" type="checkbox">

<label for="session_state">Click It!</label>
```


... the `"session_state"` value allows clicking on the `label` element to toggle `input` state of the checkbox. When combined with CSS `:checked` pseudo class this allows for powerful manipulation of page layout and styling!


Few things to keep in mind:


- an `id` attribute should be unique for a page, if two or more elements have the same `id` value then the first defined within the HTML markup will be targeted, and all others will be ignored


- multiple `label`, or other elements, may have the same `for` target but this functionality is not utilized as often


- because the `id` and `for` elements may be in any order, any depth, this may be leveraged to allow CSS to operate beyond the normal _Cascade_


> In fact any element other than `:root` and `body` are able to be modified via a strategically placed `input` element. However, beware such hacks may cause markup to become unmaintainable in the future!


---


### `assets/css/style.css`
[heading__assetscssstylecss]: #assetscssstylecss


> **[`assets/css/style.css`][branch__current__style_css]** Provides additional styling and further enhances menu presentation.


Much of the styling within this file is for visual presentation, and it is recommend to open a web-browser console to toggle various settings.


______


## Contributing
[heading__contributing]:
  #contributing
  "&#x1F4C8; Options for contributing to css-navigation-menu and web-dev-examples"


Options for contributing to css-navigation-menu and web-dev-examples


---


### Forking
[heading__forking]:
  #forking
  "&#x1F531; Tips for forking css-navigation-menu"


Start making a [Fork][css_navigation_menu__fork_it] of this repository to an account that you have write permissions for.


- Add remote for fork URL. The URL syntax is _`git@github.com:<NAME>/<REPO>.git`_...


```Bash
cd ~/git/hub/web-dev-examples/css-navigation-menu

git remote add fork git@github.com:<NAME>/css-navigation-menu.git
```


- Commit your changes and push to your fork, eg. to fix an issue...


```Bash
cd ~/git/hub/web-dev-examples/css-navigation-menu


git commit -F- <<'EOF'
:bug: Fixes #42 Issue


**Edits**


- `<SCRIPT-NAME>` script, fixes some bug reported in issue
EOF


git push fork gh-pages
```


> Note, the `-u` option may be used to set `fork` as the default remote, eg. _`git push -u fork gh-pages`_ however, this will also default the `fork` remote for pulling from too! Meaning that pulling updates from `origin` must be done explicitly, eg. _`git pull origin gh-pages`_


- Then on GitHub submit a Pull Request through the Web-UI, the URL syntax is _`https://github.com/<NAME>/<REPO>/pull/new/<BRANCH>`_


> **Warning** the source code and styling for `index.html` file are intentionally minimal!
> In other words; enhancement related Pull Requests should generally focus on `assets/css/style.css`, and bug related Pull Requests should target `index.html` file.
>
> To decrease the chances of documentation related Pull Request needing modifications before being accepted, please check the [dot-github](https://github.com/web-dev-examples/.github) repository for detailed contributing guidelines.


---


### Sponsor
  [heading__sponsor]:
  #sponsor
  "&#x1F4B1; Methods for financially supporting web-dev-examples that maintains css-navigation-menu"


Thanks for even considering it!


Via Liberapay you may <sub>[![sponsor__shields_io__liberapay]][sponsor__link__liberapay]</sub> on a repeating basis.


Regardless of if you're able to financially support projects that Web-Dev Examples maintains, please consider sharing projects that are useful with others, because one of the goals of maintaining Open Source repositories is to provide value to the community.


______


## Attribution
[heading__attribution]:
  #attribution
  "&#x1F4C7; Resources that where helpful in building this project so far."


- [GitHub -- `github-utilities/make-readme`](https://github.com/github-utilities/make-readme)


______


## License
[heading__license]:
  #license
  "&#x2696; Legal side of Open Source"


```
Pure CSS and HTML navigation menu example
Copyright (C) 2021 S0AndS0

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, version 3 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
```


For further details review full length version of [AGPL-3.0][branch__current__license] License.



[branch__current__license]:
  /LICENSE
  "&#x2696; Full length version of AGPL-3.0 License"

[branch__current__index_html]:
  /index.html
  "&#x1f578; Contains HTML5 elements that define page structure, and inline CSS3 is leveraged to provide core menu functionality"

[branch__current__style_css]:
  /assets/css/style.css
  "&#x1f58c; Provides additional styling and further enhances menu presentation"

[badge__commits__css_navigation_menu__gh_pages]:
  https://img.shields.io/github/last-commit/web-dev-examples/css-navigation-menu/gh-pages.svg

[commits__css_navigation_menu__gh_pages]:
  https://github.com/web-dev-examples/css-navigation-menu/commits/main
  "&#x1F4DD; History of changes on this branch"


[css_navigation_menu__community]:
  https://github.com/web-dev-examples/css-navigation-menu/community
  "&#x1F331; Dedicated to functioning code"

[css_navigation_menu__gh_pages]:
  https://github.com/web-dev-examples/css-navigation-menu/tree/
  "Source code examples hosted thanks to GitHub Pages!"

[badge__gh_pages__css_navigation_menu]:
  https://img.shields.io/website/https/web-dev-examples.github.io/css-navigation-menu/index.html.svg?down_color=darkorange&down_message=Offline&label=Demo&logo=Demo%20Site&up_color=success&up_message=Online

[gh_pages__css_navigation_menu]:
  https://web-dev-examples.github.io/css-navigation-menu/index.html
  "&#x1F52C; Check the example collection tests"

[issues__css_navigation_menu]:
  https://github.com/web-dev-examples/css-navigation-menu/issues
  "&#x2622; Search for and _bump_ existing issues or open new issues for project maintainer to address."

[css_navigation_menu__fork_it]:
  https://github.com/web-dev-examples/css-navigation-menu/
  "&#x1F531; Fork it!"

[pull_requests__css_navigation_menu]:
  https://github.com/web-dev-examples/css-navigation-menu/pulls
  "&#x1F3D7; Pull Request friendly, though please check the Community guidelines"

[css_navigation_menu__gh_pages__source_code]:
  https://github.com/web-dev-examples/css-navigation-menu/
  "&#x2328; Project source!"

[badge__issues__css_navigation_menu]:
  https://img.shields.io/github/issues/web-dev-examples/css-navigation-menu.svg

[badge__pull_requests__css_navigation_menu]:
  https://img.shields.io/github/issues-pr/web-dev-examples/css-navigation-menu.svg

[badge__gh_pages__css_navigation_menu__source_code]:
  https://img.shields.io/github/repo-size/web-dev-examples/css-navigation-menu


[sponsor__shields_io__liberapay]:
  https://img.shields.io/static/v1?logo=liberapay&label=Sponsor&message=web-dev-examples

[sponsor__link__liberapay]:
  https://liberapay.com/web-dev-examples
  "&#x1F4B1; Sponsor developments and projects that web-dev-examples maintains via Liberapay"

