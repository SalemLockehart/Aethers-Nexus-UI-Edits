# [Aether's](https://next.nexusmods.com/profile/Aether) Theme for Nexus Mods
These UBlockOrigin filters were created to make [Nexus Mods](https://www.nexusmods.com/)' new UI feel more like its previous iterations.

This theme attempts to waste less space by reducing font size, removing unnecessary padding, UI elements, and headers. It also removes the Popular Collections section on game pages, as I felt it took away priority from newly released mods, and collections can be accessed through the drop-down menu at the top of the site.

Additionally, some general cosmetic edits have been included, which remove the background image from Game, and Mod pages.

## Overview
This auto-updating theme utilizes UBlock Origin's Filter Lists to make layout, and cosmetic changes to Nexus Mods. It is semi-modular, allowing you to only install the filter lists you want.

There are two filter lists, each listed below:
### Main Theme (Layout Changes)
***Home Page***
* Removed the blue "Download Collections" section between Games and News & Updates
* Removed the Vortex Advertisement Footer. (Also applies to Mod Pages.)

***Game Pages***
* Removed the game title header at the top of the page, added padding for Trending Mods.
* Collections section has been removed.
* Reduced padding size between Trending and More Mods, removed icons.
* Reduced the font size of Trending and More Mods.
* Reduced the padding and removed the border between the More Mods title and the section itself.
* Increased the number of mods displayed in More Mods from four per row to five.
* Reduced the padding between mods in the More Mods section.
* Reduced the total number of mods in the More Mods section to 15. (Clicking "View more mods" will show you the 16th mod)
* Removed the padding, and border at the end of the More Mods section, between the View more mods button.

***Search Page***
* Removed the "Make mods. Earn rewards." block from the Search page.
### Cosmetic Edits (Visual Changes)
* Game images will no longer influence the background color of each game page.
* Header images will no longer influence the backgroud color of each mod page.
## Installation
If you are using a version of this theme from before it was switched over to UBlock's Filter List feature, please uninstall it before proceeding.

1. Install [uBlock Origin](https://ublockorigin.com/);
2. Open uBlock Origin's Dashboard, then navigate to "Filter Lists";
3. Scroll to the bottom of the page, and expand the "Import..." section;
4. Copy and paste either of these filter links into this section (both can be used together or separately):
  
  **Main Theme (Layout Changes)**
  ```txt
  https://raw.githubusercontent.com/SalemLockehart/Aethers-Nexus-UI-Edits/refs/heads/main/filters/aethernexustheme-main.txt
  ```
  **Cosmetic Edits (Visual Changes)**
  ```txt
  https://raw.githubusercontent.com/SalemLockehart/Aethers-Nexus-UI-Edits/refs/heads/main/filters/aethernexustheme-cosmetic.txt
  ```
5. Press "Apply changes"
6. Verify that the changes are functioning as intended on Nexus Mods.

## Preview
[Before & After Photos](https://github.com/SalemLockehart/Aethers-Nexus-UI-Edits/tree/main/Before%20%26%20After%20Pictures)

![Game Page Comparison](https://raw.githubusercontent.com/SalemLockehart/Aethers-Nexus-UI-Edits/refs/heads/main/Before%20%26%20After%20Pictures/Game%20Page%20comparision.png)
