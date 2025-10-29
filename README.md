# Xovi Extensions

This repo consists of multiple xovi (.qmd) extensions that are QoL improvements to the xochitl interface. These require qt-resource-rebuilder.so to work.

Instructions to install xovi can be found [here](https://github.com/asivery/rmpp-xovi-extensions/blob/master/INSTALL.MD). 

Download the extensions from the folder matching your reMarkable software version. 

Copy the `.qmd` files to `/home/root/xovi/exthome/qt-resource-rebuilder/` and restart xovi.

Some of the QMD files in this repo are my own and some are modifications I've made to extensions created by others in the community. Modifications will link to the original author.

Extensions have been tested only for the latest reMarkable OS version, though they may work on newer versions.

Beta releases are not tested nor supported.

## Extensions

### 1. gestures.qmd
**Original**: https://github.com/ingatellent/xovi-qmd-extensions

Add the following gestures and tap areas:
- Swipe down with three fingers to reset pan and zoom, i.e. to scroll to top of the page and zoom to 100%
- Swipe out and in from the toolbar to show/hide the toolbar - for horizontal toolbar, the swipe only works at the show toolbar button (in order not to interfere with native gestures)
- When the toolbar is hidden, tap on the bottom right to scroll down, and to change to the next page if you are already nearly at the bottom) (no scrollbar shown)
- When the toolbar is hidden, tap on the bottom left to scroll up, and to change to the previous page if you are already nearly at the top) (no scrollbar shown)

PDF links in the tap area cannot be used while the toolbar is closed, show the toolbar to restore link functionality.

**Modifications I've made**
 - Removed the 4-finger contrast filter gesture

### 2. hideDevModeIcon.qmd
Hide the developer mode icon next to the battery icon.

### 3. hideZoomIndicator.qmd
Auto-hide zoom indicator after 4 seconds (like the scrollbars).

### 4. miniLightSleep.qmd
**Original**: https://github.com/StarNumber12046/xovi-qmd-extensions

Replaces the light sleep banner with text saying "Sleeping" at the top right of the screen

**Modifications I've made**
- Changed text from "Zzz..." to "Sleeping"
- Added white background to the sleeping text

### 5. preventNotebookZoomOut.qmd
Forces all notebook pages to start at 1x zoom with optional horizontal offset. Only affects notebooks, only affects portrait orientation. Designed for the Paper Pro Move.

### 6. quickSettingsScreenshot.qmd
Adds a screenshot button to the quick settings menu.  
_See required repos for supported devices._

Requires:
- [rm-shot](https://github.com/rmitchellscott/rm-shot)
- [framebuffer-spy](https://github.com/asivery/rm-xovi-extensions)
- [xovi-message-broker](https://github.com/asivery/rm-xovi-extensions)

### 7. unlockMethodsContent.qmd
Bypass subscription check for using on-device Methods templates and documents.

## License

- **Original works** are licensed under the MIT License (see [LICENSE](LICENSE)).
- **Derivative works** retain attribution to their original authors - see individual file headers for details.
