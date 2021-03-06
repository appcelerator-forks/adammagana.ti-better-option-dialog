# Better Titanium Option Dialog

[![gitTio](http://gitt.io/badge.svg)](http://gitt.io/component/com.magana.betteroptiondialog)
[![Dependencies](https://david-dm.org/adammagana/ti-better-option-dialog/status.svg?style=flat-square)](https://david-dm.org/adammagana/ti-better-option-dialog#info=dependencies)
[![Dev Dependencies](https://david-dm.org/adammagana/ti-better-option-dialog/dev-status.svg?style=flat-square)](https://david-dm.org/adammagana/ti-better-option-dialog#info=devDependencies)

> A wrapper for Titanium's Option Dialog that makes it simpler to add option buttons.

## Demonstration

![Demonstration](demonstration.gif)

## Usage

### Installation

Download the latest distribution ZIP-file and consult the [Titanium Documentation](http://docs.appcelerator.com/titanium/latest/#!/guide/Using_a_Module) on how install it, or simply use the [gitTio CLI](http://gitt.io/cli):

```bash
gittio install com.magana.betteroptiondialog
```

### Example

```javascript
var BetterOptionDialog = require('com.magana.betteroptiondialog');

var optionDialog = BetterOptionDialog.create({
    options: [
        {
            callback: function (optionDialogEventData) {
                // Code to delete something here
            },
            destructive: true,
            title: 'Delete'
        },
        {
            callback: function (optionDialogEventData) {
                // Code to save something here
            },
            title: 'Save'
        }
    ],
    showCancel: true, // Will automatically add a cancel button to the option dialog
    title: 'Better Option Dialog!'
});

optionDialog.show();
```

## Credits

* [@smclab](https://github.com/smclab/titaniumifier) for [titaniumifier](https://github.com/smclab/titaniumifier)
* [@FokkeZB](https://github.com/FokkeZB) for inspiration for this repository's structure ([ti-html2as](https://github.com/FokkeZB/ti-html2as))

## License

This library, *betteroptiondialog*, is free software ("Licensed Software"); you can
redistribute it and/or modify it under the terms of the [GNU Lesser General
Public License](http://www.gnu.org/licenses/lgpl-2.1.html) as published by the
Free Software Foundation; either version 2.1 of the License, or (at your
option) any later version.

This library is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; including but not limited to, the implied warranty of MERCHANTABILITY,
NONINFRINGEMENT, or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
Public License for more details.

You should have received a copy of the [GNU Lesser General Public
License](http://www.gnu.org/licenses/lgpl-2.1.html) along with this library; if
not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth
Floor, Boston, MA 02110-1301 USA
