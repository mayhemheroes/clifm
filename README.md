<p align="center">
	<a href="https://github.com/leo-arch/clifm">
		<img src="https://i.postimg.cc/Gm5vxMLp/256x256c.png" alt="CliFM logo" width="160" height="160">
	</a>
</p>
<h1 align="center">CliFM</h1>
<h2 align="center">The Command Line File Manager</h2>
<h3 align="center">Fast, extensible, lightweight</h3>
<h3 align="center">Linux, Termux (Android), FreeBSD, NetBSD, OpenBSD, MacOS, Haiku, Cygwin | x86, ARM</h3>
<h4 align="center"><a
href="https://github.com/leo-arch/clifm/#floppy_disk-installation">Install</a> · <a
href="https://github.com/leo-arch/clifm/wiki">Browse the documentation</a> · <a
href="https://github.com/leo-arch/clifm/blob/master/.github/ISSUE_TEMPLATE/feature-request.md">Request feature</a> · <a
href="https://github.com/leo-arch/clifm/issues">Report bug</a></h4>

---

<p align="center">
<a href="https://github.com/leo-arch/clifm/blob/master/LICENSE"><img src="https://img.shields.io/github/license/leo-arch/clifm?color=red&style=flat"/></a>
<a href="https://github.com/leo-arch/clifm/releases"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/leo-arch/clifm"></a>
<a><img src="https://img.shields.io/github/commits-since/leo-arch/clifm/latest"></a>
<a><img src="https://img.shields.io/github/last-commit/leo-arch/clifm/master?color=blue&style=flat"/></a>
<a href="https://en.wikipedia.org/wiki/Privacy-invasive_software"><img src="https://img.shields.io/badge/privacy-✓-green?style=flat"/></a>
<a href="https://gitter.im/leo-arch/clifm"><img src="https://img.shields.io/gitter/room/leo-arch/clifm?style=flat"/></a>
<a href="https://software.opensuse.org//download.html?project=home%3Aarchcrack&package=clifm"><img src="https://img.shields.io/badge/CD-OBS-red?logo=opensuse&logoColor=white"/></a>
</p>

<p align="center">
<a href="https://github.com/leo-arch/clifm/actions/workflows/codeql-analysis.yml"><img src="https://github.com/leo-arch/clifm/actions/workflows/codeql-analysis.yml/badge.svg?branch=master"></a>
<a href="https://www.codacy.com/gh/leo-arch/clifm/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=leo-arch/clifm&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/c2c24860fce64d2aa6ca8e1dd0981d6d"/></a>
<a href="https://app.codiga.io/project/30518/dashboard"><img alt="Code grade" src="https://api.codiga.io/project/30518/status/svg"/></a>
<!---
<a href="https://bestpractices.coreinfrastructure.org/projects/4884"><img src="https://bestpractices.coreinfrastructure.org/projects/4884/badge"></a>
-->
</p>

<!---
<a href="https://lgtm.com/projects/g/leo-arch/clifm/context:cpp"><img alt="Language grade: C/C++" src="https://img.shields.io/lgtm/grade/cpp/g/leo-arch/clifm.svg?logo=lgtm&logoWidth=18"/></a>
<a href="https://codecov.io/gh/leo-arch/clifm"><img src="https://codecov.io/gh/leo-arch/clifm/branch/master/graph/badge.svg?token=YC3NIS180Z"/></a>
[![LGTM](https://img.shields.io/lgtm/grade/cpp/g/leo-arch/clifm.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/leo-arch/clifm/context:cpp)
-->

---

## Table of contents
🔸 [Brief description](#space_invader-brief-description) \
🔸 [Features](#heavy_check_mark-features) \
🔸 [Introduction video](#clapper-introduction-video) \
🔸 [What's new?](#newspaper-whats-new) \
🔸 [Installation](#floppy_disk-installation) \
🔸 [Getting started](#bulb-getting-started) \
🔸 [Support](#support) \
🔸 [License](#license) \
🔸 [Contributing](#contributing) \
🔸 [Community](#community)

---

## :space_invader: Brief description

**Clifm** is a **C**ommand **L**ine **I**nterface **F**ile **M**anager: all input and interaction is performed via commands. This is its main feature and strength.

Unlike most terminal file managers out there, indeed, **clifm** replaces the traditional TUI interface (also known as curses or text-menu based interface) by a command-line interface (CLI),<sup>1</sup> also known as REPL.<sup>2</sup>

If working with the command-line, your workflow is not affected at all, but just enriched with file management functionalities: automatic files listing, files selection, bookmarks, tags, directory jumper, directory and commands history, auto-cd and auto-open, bulk rename, TAB completion, autosuggestions, and a trash system, among [other features](#features). In this sense, **clifm** is certainly a file manager, but also a shell extension.

Briefly put, with **clifm** the command-line is always already there, never hidden :godmode: :muscle:

---
<sup>1</sup> <i>For more information about these concepts see the [resources page](https://github.com/leo-arch/clifm/wiki/Resources#gui-tui-and-cli) </i>. \
<sup>2</sup> <i>For a detailed description consult the [introductory section](https://github.com/leo-arch/clifm/wiki/Introduction#what-is-clifm) of our Wiki</i>.

---

<h4 align="center">CliFM's interface</h4>
<p align="center"><img src="https://i.postimg.cc/YC77qSLK/interface-1-7-9.png"></p>
<p align="center">We only need 7 keystrokes to move all selected files into the <i>images</i> directory</p>
<!---
<p align="center"><img src="https://i.postimg.cc/BZMv62VP/interface1-7-5.png"></p>
<p align="center"><img src="https://i.postimg.cc/Zqp4sgLK/clifm-interface8.png"></p>
--->

---

## :heavy_check_mark: Features

<details>
<summary>Click here to expand</summary>

Besides common file operations such as copy, move, remove, etc., _clifm_ provides the following features:
- Specific
  - [Really CLI-based](https://github.com/leo-arch/clifm/wiki/Introduction#main-design-and-goals). No GUI nor TUI at all, but just a command-line
  - It can run on the kernel built-in console and even on a SSH or any other remote session
  - Highly compatible with old VT102-only terminal emulators like Rxvt and Rxvt-based ones: even on a terminal with only 8 colors and no Unicode support, **clifm** will just work. [It can run even on an old DEC-VT100 terminal!](https://github.com/leo-arch/clifm/wiki/Extra#clifm-running-on-a-dec-vt100-terminal-1978)
  - [High performance](https://github.com/leo-arch/clifm/wiki/Performance). Incredibly lightweight and fast even on really old hardware
  - [Short (and even one-character) commands](https://github.com/leo-arch/clifm/wiki/Introduction#commands-short-summary)
  - [Entry list numbers (ELN's)](https://github.com/leo-arch/clifm/wiki/Common-Operations) for file names
  - [Extended color codes](https://github.com/leo-arch/clifm/wiki/Customization#colors) for file-types and -extensions
  - [Files counter](https://github.com/leo-arch/clifm/wiki/Introduction#interface) for directories and symlinks to directories
  - Privacy: Zero data collection and no connection to the outside world at all
  - Security: [Secure environment](https://github.com/leo-arch/clifm/wiki/Specifics#security) and [secure commands](https://github.com/leo-arch/clifm/wiki/Specifics#security). See also the [stealth mode section](https://github.com/leo-arch/clifm/wiki/Specifics#stealth-mode)
- Navigation and file operations
  - [Bookmarks](https://github.com/leo-arch/clifm/wiki/Common-Operations#bookmarks)
  - [File tags](https://github.com/leo-arch/clifm/wiki/Common-Operations#tagging-files)
  - [File filters](https://github.com/leo-arch/clifm/wiki/Advanced#files-filters)
  - [Files selection](https://github.com/leo-arch/clifm/wiki/Common-Operations#selection) (supports both glob and regular expressions and works even across multiple instances of the program)
  - [Files search](https://github.com/leo-arch/clifm/wiki/Common-Operations#searching) (supports both glob and regular expressions)
  - [copy(-as), move(-as)](https://github.com/leo-arch/clifm/wiki/Introduction#c-l-e-edit-m-md-r), [interactive rename](https://github.com/leo-arch/clifm/wiki/Introduction#c-l-e-edit-m-md-r), and [open-with](https://github.com/leo-arch/clifm/wiki/Introduction#ow-elnfilename-application) functions
  - [File names cleaner](https://github.com/leo-arch/clifm/wiki/Introduction#bb-bleach-elnfile--n)
  - [Autocommands](https://github.com/leo-arch/clifm/wiki/Specifics#autocommands)
  - [Auto-cd](https://github.com/leo-arch/clifm/wiki/Introduction#acd-autocd-on-off-status), [auto-open](https://github.com/leo-arch/clifm/wiki/Introduction#ao-auto-open-on-off-status), and [autols](https://github.com/leo-arch/clifm/wiki/Common-Operations#navigation)
  - [Directory jumper](https://github.com/leo-arch/clifm/wiki/Specifics#kangaroos-frecency-algorithm), similar to [autojump](https://github.com/wting/autojump), [z.lua](https://github.com/skywind3000/z.lua), and [zoxide](https://github.com/ajeetdsouza/zoxide)
  - [Virtual directories](https://github.com/leo-arch/clifm/wiki/Advanced#virtual-directories)
  - [Fastback - Quickly change to any parent directory](https://github.com/leo-arch/clifm/wiki/Introduction#fastback)
  - [A built-in resource opener](https://github.com/leo-arch/clifm/wiki/Specifics#resource-opener) (supports regular expressions and is able to discern between GUI and non-GUI environments)
  - [A built-in Freedesktop-compliant trash system](https://github.com/leo-arch/clifm/wiki/Common-Operations#trashing-files)
  - [Up to eight workspaces](https://github.com/leo-arch/clifm/wiki/Specifics#workspaces)
  - [Eleven sorting methods](https://github.com/leo-arch/clifm/wiki/Introduction#st-sort-method-rev)
  - [Bulk operations](https://github.com/leo-arch/clifm/wiki/Advanced#bulk-operations): rename, create, remove, and create symbolik links in bulk
  - [Files encryption/decryption (plugin)](https://github.com/leo-arch/clifm/wiki/Advanced#plugins)
  - [Copy files to your smart phone (plugin)](https://github.com/leo-arch/clifm/wiki/Advanced#plugins)
  - [Archiving and compression](https://github.com/leo-arch/clifm/wiki/Advanced#archives) support (including Zstandard and ISO 9660)
  - [Symlinks editor](https://github.com/leo-arch/clifm/wiki/Introduction#c-l-e-edit-m-md-r)
  - [Remote file systems management](https://github.com/leo-arch/clifm/wiki/Introduction#net-name-edit-m-mount-name-u-unmount-name)
  - [Mount/unmount storage devices](https://github.com/leo-arch/clifm/wiki/Introduction#media)
  - [Advanced Copy](https://github.com/leo-arch/clifm/wiki/Advanced#cpmv-with-a-progress-bar) support (just `cp` and `mv` with a nice progress bar)
  - Directory history map to keep in sight previous, current, and next entries in the directory history list
- Shell
  - [Auto-suggestions](https://github.com/leo-arch/clifm/wiki/Specifics#auto-suggestions)
  - [TAB completion](https://github.com/leo-arch/clifm/wiki/Specifics#expansions-completions-and-suggestions), with _fzf_ integration (including [file previews](https://github.com/leo-arch/clifm/wiki/Advanced#files-preview))
  - [Syntax highlighting](https://github.com/leo-arch/clifm/wiki/Specifics#syntax-highlighting)
  - [Warning prompt for invalid command names](https://github.com/leo-arch/clifm/wiki/Customization#the-warning-prompt)
  - [Fused parameters for ELN's](https://github.com/leo-arch/clifm/wiki/Introduction#fused-parameters)
  - [Fuzzy completion for file names and paths](https://github.com/leo-arch/clifm/wiki/Specifics#fuzzy-match)
  - [Wildcards expansion via <kbd>TAB</kbd>](https://github.com/leo-arch/clifm/wiki/Introduction#filter-files-with-the-tab-key) (`s *.[ch]<TAB>`)
  - [File types expansion via <kbd>TAB</kbd>](https://github.com/leo-arch/clifm/wiki/Introduction#filter-files-with-the-tab-key) (`=l<TAB>` to list all symlinks in the current dir)
  - Bash-like quoting system
  - Shell commands execution
  - Sequential and conditional commands execution
  - [Directory](https://github.com/leo-arch/clifm/wiki/Introduction#b-back-h-hist-clear-eln) and [commands](https://github.com/leo-arch/clifm/wiki/Introduction/#commands-history) history
  - [Glob and regular expressions](https://github.com/leo-arch/clifm/wiki/Advanced#wildcards-and-regex) (including inverse matching)
  - [Aliases](https://github.com/leo-arch/clifm/wiki/Customization#aliases)
  - [Logs](https://github.com/leo-arch/clifm/wiki/Introduction#log-clear-on-off-status)
  - [Prompt and profile commands](https://github.com/leo-arch/clifm/wiki/Customization#profile-and-prompt-commands) (run commands with each new prompt or at program startup)
- Modes
  - [Stealth mode](https://github.com/leo-arch/clifm/wiki/Specifics#stealth-mode), also known as incognito or private mode
  - [Light mode](https://github.com/leo-arch/clifm/wiki/Specifics#light-mode) (just in case it is not fast enough for you)
  - [Resource opener](https://github.com/leo-arch/clifm/wiki/Specifics#using-clifm-as-a-standalone-resource-opener)
  - [Disk usage analyzer mode](https://github.com/leo-arch/clifm/wiki/Specifics#disk-usage-analyzer)
  - [Files lister (ls-mode)](https://github.com/leo-arch/clifm/wiki/Advanced#files-lister-ls-mode)
- Customization
  - [User profiles](https://github.com/leo-arch/clifm/wiki/Specifics#profiles)
  - [Customizable keyboard shortcuts](https://github.com/leo-arch/clifm/wiki/Customization#keybindings)
  - [Theming support](https://github.com/leo-arch/clifm/wiki/Customization#theming) (more than a dozen color schemes)
  - [Prompt customization](https://github.com/leo-arch/clifm/wiki/Customization#the-prompt)
  - [Four customizable keybindings for custom plugins](https://github.com/leo-arch/clifm/wiki/Customization#keybindings)
  - [Compile features in/out](https://github.com/leo-arch/clifm/blob/master/src/README.md#compiling-features-inout)
- Misc
  - [Plugins](https://github.com/leo-arch/clifm/wiki/Advanced#plugins)
  - [File previews](https://github.com/leo-arch/clifm/wiki/Advanced#files-preview) (via TAB completion!)
  - [Icons support](https://github.com/leo-arch/clifm/wiki/Advanced#icons-smirk), including emoji-icons :smirk:
  - [Git integration](https://github.com/leo-arch/clifm/wiki/Advanced#git-integration)
  - [Desktop notifications](https://github.com/leo-arch/clifm/wiki/Specifics#desktop-notifications)
  - Unicode suppport
  - Disk usage
  - [CD on quit](https://github.com/leo-arch/clifm/wiki/Advanced#cd-on-quit) and [file picker](https://github.com/leo-arch/clifm/wiki/Advanced#file-picker) functions
  - [A built-in pager](https://github.com/leo-arch/clifm/wiki/Introduction#pg-pager-on-off-status-num) for files listing
  - Read and list files from [STDIN (standard input)](https://github.com/leo-arch/clifm/wiki/Advanced#standard-input)
<h4 align="center"><br><i>Auto-suggestions in action</i></h4>
<p align="center"><img src="https://i.postimg.cc/1XSKBRh8/suggestions.gif"></a></p>

---
For a detailed explanation of each of these features, follow the corresponding links or consult the [Wiki](https://github.com/leo-arch/clifm/wiki).
</details>

---

## :clapper: Introduction video

[![Alt text](https://img.youtube.com/vi/CJmcisw9F90/0.jpg)](https://www.youtube.com/watch?v=CJmcisw9F90)

<!---
<details>
<summary>Watch me fly!</summary>

<h3 align="center"><br><i>Did I say it's fast?</i></h3>
<p align="center"><a href="https://mega.nz/embed/J8hEkCZZ#fGp0JtcDvFIWKmTc4cOp0iMrWRlbqs99THg8F7EmQWI"><img src="https://i.postimg.cc/CKx6zrvL/vid-thumb.png"></a></p>

Music: "Quad Machine", by [Sonic Mayhem](https://en.wikipedia.org/wiki/Sascha_Dikiciyan) \
**Note**: Icons and files preview depend on third-party software. Consult the [icons](https://github.com/leo-arch/clifm/wiki/Advanced#icons-smirk) and [files preview](https://github.com/leo-arch/clifm/wiki/Advanced#files-preview) sections.

</details>
-->

---

## :newspaper: What's new?
<details>
<summary>Click here to expand</summary>

* `Development`:
  - **NEW**: `s:` works now like `sel` keyword, to be in line with `t:` (for tags) and `b:` (for bookmarks). Consult the [Files selection](https://github.com/leo-arch/clifm/wiki/Common-Operations#selection) section.
  - **NEW**: The `:b` construct was removed. `b:` now lists bookmark names instead of paths. `b:mybm` expands to the path pointed to by the bookmark named `mybm`. The `ExpandBookmarks` option (config file) is now deprecated, just as the bookmarks suggestions strategy (in the `SuggestionStrategy` option). See the [Bookmarks](https://github.com/leo-arch/clifm/wiki/Common-Operations#bookmarks) section.
  - **NEW**: Bookmarks can be created directly from the command line, without an interactive prompt: `bm add FILE BM_NAME`.
  - **NEW**: [Rename profiles via the `rename` subcommand](https://github.com/leo-arch/clifm/wiki/Introduction#pf-prof-profile-ls-list-set-add-del-profile-rename-profile-new_name)
  - **NEW**: [`oc`, a files ownership editor](https://github.com/leo-arch/clifm/wiki/Introduction#oc-elnfile-)
  - **NEW**: Get list of commands and a brief description via `cmd<TAB>` 
  - **NEW**: [Suggest a brief description for internal commands](https://github.com/leo-arch/clifm/wiki/Specifics#auto-suggestions)
  - **NEW**: Set a custom selections file via the `--sel-file` flag
* `version 1.9 (Sharptooth)`:
  - [Improved fuzzy suggestions/completions for file names and paths](https://github.com/leo-arch/clifm/wiki/Specifics#auto-suggestions)
  - [Automatic expansion for bookmarks, file type, and MIME type filters](https://github.com/leo-arch/clifm/wiki/Advanced#grouping-files-via-automatic-expansion)
  - [Private workspace settings](https://github.com/leo-arch/clifm/wiki/Specifics#workspace-settings)
  - [Run autocommands based on workspaces, and not just on paths](https://github.com/leo-arch/clifm/wiki/Specifics#autocommands)
  - [Run the pager based on the current amount of files](https://github.com/leo-arch/clifm/wiki/Introduction#pg-pager-on-off-status-num)
  - Files counter for directories in long view mode
  - [Filter files by file type](https://github.com/leo-arch/clifm/wiki/Introduction#ft-filter-unset-regexfile-type-char)
  - [Filter files by MIME type](https://github.com/leo-arch/clifm/wiki/Advanced/#quickly-filtering-files-with-the-tab-key)
  - [`pc`, a file permissions editor](https://github.com/leo-arch/clifm/wiki/Introduction#pc-elnfile-)
  - `cd -` works now just like in most shells
  - The [`view` command](https://github.com/leo-arch/clifm/wiki/Introduction#view-edit-app) can now select files via <kbd>TAB</kbd>
  - Launch the [`view` command](https://github.com/leo-arch/clifm/wiki/Introduction#view-edit-app) via <kbd>Alt+-</kbd>
  - Use `--fzfpreview-hidden` to start the preview window hidden (toggle via <kbd>Alt-p</kbd>)
* `version 1.8 (Otis)`:
  - If upgrading from a previous version (optional, but recommended):
    - <kbd>F7</kbd> opens now shotgun's configuration file (instead of the jump database file). Update `keybindings.clifm`: removing the file and restarting is enough. Manually: run `kb edit` and then replace `open-jump-db:\e[18~` by `open-preview:\e[18~`.
    - New specific options to control the files preview window. Add the following options to the `FzfTabOptions` line in your theme file (via the `cs edit` command) or just copy the theme file from the data directory (usually `/usr/local/share/clifm/colors`): `--bind alt-p:toggle-preview,change:top,alt-up:preview-page-up,alt-down:preview-page-down --preview-window=wrap,border-left --color="border:7:dim"`.
  - [`clifmimg` plugin, for image previews](https://github.com/leo-arch/clifm/tree/master/misc/tools/imgprev#image-previews)
  - [`view` command, to preview files in full screen](https://github.com/leo-arch/clifm/wiki/Introduction#view-edit-app)
  - [TAB completion with file previews](https://github.com/leo-arch/clifm/wiki/Specifics#tab-completion-with-file-previews)
  - [Shotgun, a built-in files previewer](https://github.com/leo-arch/clifm/wiki/Advanced#shotgun)
  - Improved Unicode support for the suggestions system
  - Flat-view for the [`fzfsel` plugin](https://github.com/leo-arch/clifm/wiki/Advanced#plugins) via the `-f` option
  - [Improved VT100 compatibility via the `--vt100` switch](https://github.com/leo-arch/clifm/wiki/Extra#clifm-running-on-a-dec-vt100-terminal-1978)
  - [Cygwin support](https://github.com/leo-arch/clifm/wiki/Introduction#small_blue_diamond-d-cygwin)
  - Improved performance/portability of the suggestions system: no more slow/non-portable `CPR`-`CUP` [escape sequences](https://www.xfree86.org/current/ctlseqs.html)! These were replaced by 100% made in-house cursor position calculation plus basic/portable escape sequences: `CUU`, `CUD`, `CUF`, and `CUB`.
* `version 1.7 (Elaine)`:
  - [Configuration files renamed from `.cfm` to `.clifm`](https://github.com/leo-arch/clifm/wiki/Specifics#new-extension-for-configuration-files) (avoid conflict with [ColdFusion](https://en.wikipedia.org/wiki/ColdFusion_Markup_Language) files)
  - <kbd>Ctrl-l</kbd> added for screen refresh
  - `cc` command removed to avoid conflicts with `/bin/cc` (use `colors` instead)
  - `--std-tab-comp` option renamed to `--stdtab` (to match `--fzytab` and `--smenutab` options)
* `version 1.6 (Guybrush)`:
  - ELN's color defaults now to cyan
  - `--no-folders-first` and `--folders-first` options renamed to `--no-dirs-first` and `--dirs-first` respectively. In the same way, the `folders-first` command was renamed to `dirs-first`.
  - `PromptStyle` option renamed as `Notifications` (taking `true` and `false` as values)
* `version 1.5 (Nano)`:
  - `Prompt`, `WarningPromptStr`, `DividingLine`, and `FfzTabOptions` options were moved from the config file to the color scheme file to get a **centralized and single theming file**. However, to keep backwards compatibility, the old location is still recognized. If any of these options is found in the color scheme file, values taken from the main configuration file will be overriden.
  - The [warning prompt](https://github.com/leo-arch/clifm/wiki/Customization#the-warning-prompt) color is set now via escape codes (exactly as the regular prompt). The `wp` color code is used now only for the _input text color_ of the warning prompt.
* `version 1.4 (Alma)`:
  - In order to make _Lira_ more powerful (it can now match entire file names instead of just file extensions) it was necessary to introduce [a little syntax modification](https://github.com/leo-arch/clifm/wiki/Specifics#syntax) in its configuration file.

</details>

For more details consult the [changelog file](https://github.com/leo-arch/clifm/blob/master/CHANGELOG).

---

## :floppy_disk: Installation

### Packaged versions

<details>
<summary>Packaging status <a href="https://repology.org/project/clifm/versions"><img src="https://repology.org/badge/tiny-repos/clifm.svg" alt="Packaging status"></a></summary>
<a href="https://repology.org/project/clifm/versions">
    <img src="https://repology.org/badge/vertical-allrepos/clifm.svg" alt="Packaging status">
</a>
</details>

If running on Linux, [binary packages](https://software.opensuse.org//download.html?project=home%3Aarchcrack&package=clifm) are available for most major distributions.

### Installing from source (Linux/BSD)

**Note**: Dependencies are most likely already satisfied, but in any case consult the [dependencies section](https://github.com/leo-arch/clifm/wiki/Introduction#1-satisfy-dependencies).

```sh
git clone https://github.com/leo-arch/clifm.git
cd clifm
sudo make install
```

For more information/supported platforms consult the [installation page](https://github.com/leo-arch/clifm/wiki/Introduction#installation).

---

## :bulb: Getting started

To start using **clifm** _you don't need to learn anything new_: the usual shell commands will just work. However, there is much more than just shell commands... \
✓ The `help` command gives you a quick introduction to **clifm**: once in the **clifm** prompt, enter `help` or `?`. \
✓ Type `cmd<TAB>` to get the list of available commands and a brief description (since version 1.9.2). \
✓ Type `help <TAB>` to get the list of available _help topics_. Select the one you want and press <kbd>Enter</kbd>. \
✓ To jump into the **COMMANDS** section in the [manpage](https://github.com/leo-arch/clifm/blob/master/misc/clifm.1.pdf), simply enter `cmd` or press <kbd>F2</kbd>. \
✓ Press <kbd>F1</kbd> to access the full manpage and <kbd>F3</kbd> to access the keybindings help-page. \
✓ To get help about some specific command just type `CMD -h`. For instance, `s -h`.

You can also take a look at some of these [basic usage-examples](https://github.com/leo-arch/clifm/wiki/Common-Operations#basic-usage-examples) to get you started. \
For a complete description please consult our [Wiki](https://github.com/leo-arch/clifm/wiki).

---

## Support

**Clifm** is C99 and POSIX-1.2008 compliant (if compiled with the `_BE_POSIX` flag). Consult the [compilation page](https://github.com/leo-arch/clifm/blob/master/src/README.md#5-compilation).\
It works on Linux, Termux (Android), FreeBSD, NetBSD, OpenBSD, MacOS, Haiku, and Cygwin, on x86 and ARM architectures.

---

## License
This project is licensed GPL version 2 (or later). \
See the [LICENSE file](https://github.com/leo-arch/clifm/blob/master/LICENSE) for details.

---

## Contributing
Yes. Please see our [contribution guidelines](https://github.com/leo-arch/clifm/blob/master/CONTRIBUTING.md) for details.
[![Translation status](https://hosted.weblate.org/widgets/clifm/-/clifm/svg-badge.svg)](https://hosted.weblate.org/engage/clifm/?utm_source=widget) at Hosted Weblate.

---

## Community
Join our [Gitter discussion room](https://gitter.im/leo-arch/clifm) and let us know what you think: ideas, comments, observations and questions are always welcome. \
The [Discussions section](https://github.com/leo-arch/clifm/discussions) of this repo is also open to input.
