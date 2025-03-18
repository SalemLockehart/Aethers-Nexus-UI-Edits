# Aether's Theme for Nexusmods
These UBlockOrigin filters were created to make [Nexus Mods](https://www.nexusmods.com/)' new UI feel more like its previous iterations.

They attempt to waste less space by reducing font size, removing unnesecary padding, UI elements, and headers. They also remove the Popular Collections and Media sections on game pages, as I felt they took away priority from newly released mods, and they can be accessed through the drop down menus at the top of the site.

Additionally, some general cosmetic edits have been included, which remove the background image from Game, and Mod pages, and also fix a cosmetic issue with the upload button at non-standard browser zoom levels.

### Installation
* Install [uBlock Origin](https://ublockorigin.com/);
* Open uBlock Origin's Dashboard, then navigate to "My Filters"
* Copy the filters from this github repository, and paste them into your filters page.
* Press "Apply changes"
* Verify that the changes are functioning as intended on Nexus Mods.

```txt
! Aether's Theme for Nexus Mods
! MIT License | Copyright (c) 2025 Salem Lockehart

! ------- Main Page
! Removed the blue "Download Collections" section between Games and News & Updates
www.nexusmods.com##.collections-banner-outer-wrapper-trigger
! Removed the Vortex Advertisement Footer. (Also applies to Mod Pages.)
www.nexusmods.com###rj-vortex

! ------- Game Page
! Removed the game title header at the top of the page.
www.nexusmods.com##.pt-4.pb-6
! Removed the divider block in the middle of the Trending Mods section.
www.nexusmods.com##.sm\:block.w-full.hidden.border-stroke-weak
! Popular Collections and Media sections have been removed.
www.nexusmods.com##section.pt-20:has-text(Popular Collections)
www.nexusmods.com##section.pt-20:has-text(Media)
! Reduced padding size between Trending and More Mods.
www.nexusmods.com##.pt-8.pb-20:style(padding-top: 1rem !important)
www.nexusmods.com##.pt-20:style(padding-top: 1.5rem !important)
! Reduced the font size of Trending and More Mods.
www.nexusmods.com##.gap-x-2.items-center.flex.text-neutral-strong.typography-heading-sm:style(font-size: .875rem !important)
! Reduced the padding and removed the border between the More Mods title and the section itself.
www.nexusmods.com##.pt-4.border-t.border-stroke-weak:style(padding-top: 0rem !important)
www.nexusmods.com##.pt-4.border-t.border-stroke-weak:style(border-top-width: 0px !important)
! Increased the number of mods displayed in More Mods from four per row to five.
www.nexusmods.com##.mods-grid:style(grid-template-columns: repeat(auto-fill, minmax(14rem, 1fr)) !important)
! Reduced the padding between mods in the More Mods section.
www.nexusmods.com##.mods-grid:style(column-gap: .7rem !important)
www.nexusmods.com##.mods-grid:style(row-gap: .7rem !important)
! Reduced the total number of mods in the More Mods section to 15. (Clicking "View more mods" will show you the 16th mod)
www.nexusmods.com##div.rounded.flex-col.min-h-\[28rem\].flex.bg-surface-low.group\/mod-tile.\@container\/mod-tile:nth-of-type(16)
! Removed the padding, and border at the end of the More Mods section, between the View more mods button.
www.nexusmods.com##.pt-6.border-t.border-stroke-weak:style(padding-top: 0rem !important)
www.nexusmods.com##.pt-6.border-t.border-stroke-weak:style(border-top-width: 0px !important)

! ------- Search/"Mods" Page
! Removed the "Make mods. Earn rewards." block.
www.nexusmods.com##.sm\:block.p-4.bg-cover.border.rounded-lg.hidden.mt-4.bg-creator-weak.border-creator-subdued

! ------- General Cosmetic Edits
! Remove Orange Upload Button Border (Fixes the button displaying incorrectly at non-standard browser zoom levels.)
www.nexusmods.com##.hover\:\!ring-primary-strong.\!ring-primary-strong.hover\:text-neutral-strong.text-neutral-moderate.hover\:ring-stroke-strong.ring-stroke-moderate.ring-1.hover-overlay.cursor-pointer.min-w-24.px-3.min-h-9.before\:rounded.rounded.items-center.justify-center.flex.\[\&\>\*\:first-child\]\:relative.whitespace-nowrap.transition.relative:style(--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color) !important)
! Game images will no longer influence the background color of each game page.
www.nexusmods.com##.absolute.inset-0.overflow-hidden
! Header images will no longer influence the backgroud color of each mod page.
www.nexusmods.com##:root:style(--body-background-image: none !important;)
```
### Preview
![Main Page](https://github.com/SalemLockehart/Aethers-Nexus-UI-Edits/blob/main/Before%20&%20After%20Pictures/Main%20Page%20After.jpg?raw=true)
![Game Page](https://github.com/SalemLockehart/Aethers-Nexus-UI-Edits/blob/main/Before%20&%20After%20Pictures/Game%20Page%20After.jpg?raw=true)
![Mod Page](https://github.com/SalemLockehart/Aethers-Nexus-UI-Edits/blob/main/Before%20&%20After%20Pictures/Mod%20Page%20After.png?raw=true)
![Search Page](https://github.com/SalemLockehart/Aethers-Nexus-UI-Edits/blob/main/Before%20&%20After%20Pictures/Search%20Page%20After.png?raw=true)
