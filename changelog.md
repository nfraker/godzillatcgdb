# Changelog
## 2.2.1
- Minor Features:
    - Refreshed card database to add 43 missing cards from web sources [Issue #52](https://github.com/nfraker/godzillatcgdb/issues/52)
    - Implemented tournament restrictions for Oxygen Destroyer, Satsuma / Shin Combo [Issue #56](https://github.com/nfraker/godzillatcgdb/issues/56)
    - Improved deck builder UX for desktop and mobile users [Private #22](https://github.com/nfraker/GTCGDB/issues/22), [Private #30](https://github.com/nfraker/GTCGDB/issues/30)
- Bug Fixes:
    - Cleaned up Z-Index values for modals and shades/drawers
    - Resolved issue with rank not rendering correctly in javascript tooltips 
## 2.2.0
- Major Features:
    - Added ability to copy public and owned decks [Issue #22](https://github.com/nfraker/godzillatcgdb/issues/22)
    - Added Deck History Backfill & Screenshots background process for administrators [Issue #47](https://github.com/nfraker/godzillatcgdb/issues/47)
    - Connected "Next" and "Previous" card navigation buttons dynamically to active search results
- Minor Features:
    - Standardized UI touch target sizes for mobile accessibility across the application [Issue #46](https://github.com/nfraker/godzillatcgdb/issues/46)
    - Improved card image pre-loading to prevent page jumping during variant animations
    - Added smooth horizontal swipe animation for navigating card variants on mobile
    - Standardized modal "Submit" / "Done" buttons across the application for improved UX
- Bug Fixes:
    - Fixed Isotope grid crash ("Cannot read properties of null") when rapidly clicking collection or search filters [Issue #16](https://github.com/nfraker/GTCGDB/issues/16)
    - Fixed broken full-size image modal click handlers on virtual lazy-loaded collection cards
    - Fixed bug causing horizontal layout overflow for some stacked search result grids
## 2.1.1
- Bug Fixes:
    - Fixed infinite scroll javascript bug in decks list
    - Fixed search filters for deck list
    - Fixed form fields in search page that were not resizing responsively
    - Fixed button CSS so selected state is visible
## 2.1.0
- Major Features:
    - Upgraded to Bootstrap 5 [Issue #44](https://github.com/nfraker/godzillatcgdb/issues/44)
    - Merged cards into "base" and "variant" hierarchy [Issue #45](https://github.com/nfraker/godzillatcgdb/issues/45)
    - Add screenshot export when deck is saved for use in opengraph [Issue #20](https://github.com/nfraker/godzillatcgdb/issues/20)
    - Add card draw simulator [Issue #18](https://github.com/nfraker/godzillatcgdb/issues/18)
- Minor Features:
    - Changed out sparkle effect with a rainbow foil that is less CPU intensive
    - Migrated img assets to S3 and Cloudfront for more resource efficient distribution
    - Refactored logic checks for one-off card rule exemptions to use array of parent_id values
- Bug Fixes:
    - Fixed issue with three-color cards not being properly calculated for deck list
    - Fixed horizontal rendering of Godzilla Earth and Token cards
    - Made password fields "Nullable" in User model to ignore blank passwords when editing user profile
    - Restored flash banners notifying users of CRUD actions
    - Fixed decks being flagged as "Resonance" even when they aren't
    - Centered isotope grids
    - Fixed odd whitespacing issues found throughout the site
## 2.0.0
- Major features:
    - Upgraded underlying infrastructure (Laravel, PHP, MySQL, JQuery) to the latest major versions of each [Issue #39](https://github.com/nfraker/godzillatcgdb/issues/39)
    - Added Set 4: Endless Wars [Issue #41](https://github.com/nfraker/godzillatcgdb/issues/41)
    - Updated Bulkzilla to comply with new "Common or Uncommon" rule change [Issue #40](https://github.com/nfraker/godzillatcgdb/issues/40)
- Bug Fixes:
    - Corrected monster deck trait chain to accurately reflect comp rules
    - Updated list of "unlimited" count cards to include EBP03 and EBP04 releases
## 1.3.0
- Major features:
    - Added Set 3: Resonance of Rivals. Also included a handful of new promo cards that have been announced in the last few months. [Issue #10](https://github.com/nfraker/godzillatcgdb/issues/10)
    - Added support for site themes, along with a Dark Mode theme. Change your preferred site theme from the Account Management screen. [Issue #21](https://github.com/nfraker/godzillatcgdb/issues/21)
    - Rebuilt the collection management screen to make it a visual interface, and enable sorting/filtering cards for ease of management.
        - NOTE: For the time being Wanted and For Trade lists have been removed until we figure out what we want to do with them.
    - Added a CMS to the backend to support future feature development. [Issue #3](https://github.com/nfraker/godzillatcgdb/issues/3)
- Bug fixes:
    - Fixed an issue with the main deck color rule validation incorrectly triggering on Resonance cards [Issue #25](https://github.com/nfraker/godzillatcgdb/issues/25)
    - Fixed an issue with the collection manager not saving records properly when the count is equal to 0. [Issue #1](https://github.com/nfraker/godzillatcgdb/issues/1)
## 1.2.0
- Major features:
    - Refactored deck builder to behave more intuitively
    - Refactored visual layout view and added photo export function
    - Refactored textual layout view for use as pdf printout decklist function [Issue #8](https://github.com/nfraker/godzillatcgdb/issues/8), [Issue #17](https://github.com/nfraker/godzillatcgdb/issues/17)
    - Added analysis view to deck viewer functionality [Issue #7](https://github.com/nfraker/godzillatcgdb/issues/7)
    - Added support for variant play format validation [Issue #16](https://github.com/nfraker/godzillatcgdb/issues/16)
    - Added support for Resonance leader rules releasing in set 3 [Issue #12](https://github.com/nfraker/godzillatcgdb/issues/12)
## 1.1.1
- Major bug fixes:
    - "Star" button automatically adds 1 to monster card count [Issue #15](https://github.com/nfraker/godzillatcgdb/issues/15)
    - Fixed card URLs to use the card's ID instead of an internal database value [Issue #14 part 1](https://github.com/nfraker/godzillatcgdb/issues/14)
    - Fixed page preview embedding in other webpages [Issue #14 part 2](https://github.com/nfraker/godzillatcgdb/issues/14)
- Minor bug fixes:
    - Improved traceability of page titles
    - Improved SEO keywords and robot text
    - Pulled Set 3 buttons until 1.2.0 is released
## 1.1.0
- Major features:
    - Advanced search filter for deck editor [Issue #6](https://github.com/nfraker/godzillatcgdb/issues/6)
    - Comprehensive deck construction validator [Issue #2](https://github.com/nfraker/godzillatcgdb/issues/2)
    - Updating visual deck list for more clarity, making default view
    - Deck editor sidebars collapsible to clear space for construction
- Major bug fixes:
    - Fixed hard-coded urls in some forms
    - Separated deck logic check for main vs monster decks
    - Refactored several layout and UI inconsistencies
## 1.0.1
- Updated search to allow Invade Zone and Rank as usable filters
- Fixed "TOKEN" rarity in search
- Minor tweaks for layout for linkbacks and proper Toho copyright
- Corrected Rank rendering for Monster cards in Deck Maker
- Refreshed Card Editor drop-downs to include EBP02 properties
- Added the Godzilla Fest 2025 special release card collection
## 1.0.0
- Initial commit of the godzillatcgdb.com site. Major features are as follows:
    - Manage collection with designations for cards owned, cards wanted, and cards for trade
    - Show your collection as a profile page that is organized automatically using [Isotope](https://isotope.metafizzy.co/)
    - Sparkly visual effect on cards that are designated as having a holofoil finish
    - Construct decks with basic card breakdowns by color and type
    - Validate deck legality by checking card count of the Monster and Main decks, and per-card count
    - Set decks as Public or Private, and search decks that have been made public by other users
    - Like cards and decks
    - Comment threads for discussing decks with other users
    - Direct Messaging between users
- Known bugs at launch time are as follows:
    - Issues with collection screen not deleting cards out of the collection, and not accurately reflecting the cards wanted/for-trade - [Issue #1](https://github.com/nfraker/godzillatcgdb/issues/1)
    - Issue with deck construction rules not validating *all* constraints - [Issue #2](https://github.com/nfraker/godzillatcgdb/issues/2)
