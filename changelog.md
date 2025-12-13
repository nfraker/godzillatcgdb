# Changelog
## 1.1.1
- Major bug fixes:
    - "Star" button automatically adds 1 to monster card count　[Issue #15](https://github.com/nfraker/godzillatcgdb/issues/15)
    - Fixed card URLs to use the card's ID instead of an internal database value [Issue #14](https://github.com/nfraker/godzillatcgdb/issues/14)
    - Fixed page preview embedding in other webpages
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
