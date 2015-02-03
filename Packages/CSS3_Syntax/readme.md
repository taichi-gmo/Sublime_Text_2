CSS3_Syntax
===========

## Announcement: For ST3 users, this package has been replaced by [CSS3](https://github.com/y0ssar1an/CSS3). This package will be removed some time after Sublime Text 3 is released.

## Features
* __Comprehensive__: near complete support for CSS3, based on the latest draft
  specs, support for many vendor-prefixed CSS extensions (e.g. -moz-, -ms-,
  -webkit-)
* __Forward-looking__: support for upcoming features like variables, CSS
  animation, and @supports
* __Modern__: deprecated or obsolete parts of CSS are flagged as such
* __Faithful__: extremely close adherence to the W3C specification, with minor deviations
  due to technical limitations (for non-trivial deviations read [below](https://github.com/y0ssar1an/CSS3_Syntax#deviations-from-the-spec))

## Installation
1. [Install Package Control](https://sublime.wbond.net/installation)
2. Mac: `cmd+shift+p` → Package Control: Install Package → CSS3 Syntax<br>
   Windows/Linux: `ctrl+shift+p` → Package Control: Install Package → CSS3 Syntax

After you've installed the plugin, open any CSS file and set the syntax to CSS.
* Mac: `cmd+shift+p` → Set Syntax: CSS3<br>
* Windows/Linux: `ctrl+shift+p` → Set Syntax: CSS3

### Set CSS3 Syntax as Default
* *WARNING: This may break extensions that only recognize the default CSS syntax,
  such as Autoprefixr. A workaround, [shown here](http://www.chriseisenbraun.com/news/autoprefixer-not-working-in-sublime-text-3-try-this-one-weird-trick-), is to switch the syntax
  back to CSS when you want to run Autoprefixr.*

1. Open a CSS file in Sublime Text
2. Navigate to View → Syntax → Open all with current extension as... → CSS3

After these steps, any CSS file you open in the future will be highlighted using CSS3 Syntax.

## Limitations
* No support for the following prefixes

<table>
    <tr>
        <td>-ah-</td>
        <td>-apple-</td>
        <td>-atsc-</td>
        <td>-hp-</td>
        <td>-ibooks-</td>
    </tr>
    <tr>
        <td>-khtml-</td>
        <td>-mso-</td>
        <td>-o-</td>
        <td>-prince-</td>
        <td>-rim-</td>
    </tr>
    <tr>
        <td>-ro-</td>
        <td>-tc-</td>
        <td>-weasy-</td>
        <td>-xv-</td>
        <td></td>
    </tr>
</table>

* Incomplete support for vendor-prefixed CSS extensions (we're adding
  more as we find them)

## Deviations from the Spec
### All Properties Must End with a Semicolon
CSS doesn't require this, but it's a good practice. Semicolons help the
highlighter distinguish properties and values. Without a semicolon, the
highlighting could be off.

  ![alt text](https://github.com/y0ssar1an/CSS3-Syntax/raw/master/screenshots/semicolon.png "Comparison between using semicolons or not.")

### All Properties Must be Written in Lowercase
The spec says that HTML tags, properties, values, function names, and more
should be matched case-insenstively. However, this syntax highlighter only
matches lowercase text. If this bothers enough people, we can work to include
matching uppercase text as well.

  ![alt text](https://github.com/y0ssar1an/CSS3-Syntax/raw/master/screenshots/case.png "Comparison between uppercase and lowercase css.")
