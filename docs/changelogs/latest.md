## Changelog

### New Features


### Feature Updates

- Farm animal's age is spoken in days if it is less than a month old.
- Animal's info include the baby and hungry statuses.
- Animal purchase menu:
    - The menu will now speak the "Select Building" prompt along with the animal's colour.
    - It will also speak the animal names as they are shown. Previously, it spoke white cow as opposed to what's shown, dairy cow.
- Added custom names support for items. This can be used to have separate names for items with same names (like for jungle decals purchasable in Luau). At the moment the scope is only at the inventory level or wherever InventoryUtils is used to get the plural form of a name.

### Bug Fixes

- Removed duplicate entries of entrances in bath house women's locker room
- Updated location of soup pot in Luau festival
- Fixed glitchiness in Pierre's shop in the Luau festival; #318
- Fixed other player's mail boxes showing up in buildings category
- Fix duplicate animal category and out of bounds animals being tracked in farms.

### Translation Changes

- New(en.ftl): `event_tile-luau-pierre_booth` with English value `Pierre's Booth`
- Modified(en.ftl): `npc-farm_animal_info` added `is_hungry`, `is_baby` and `is_age_in_days` attributes, look [here for updated english translation](https://github.com/khanshoaib3/stardew-access/blob/a33d90157baa532e09f45d72bed91ff53a601649/stardew-access/i18n/en.ftl#L333-L348)
- New(en.ftl): `tile-town-bookseller` with english value `Bookseller`
- Removed(static_tiles.en.ftl): `static_tile-town-bookseller`
- Modified(menu.en.ftl): `menu-animal_query-animal_info` added `is_age_in_days` attribute, look [here for updated english translation](https://github.com/khanshoaib3/stardew-access/blob/a33d90157baa532e09f45d72bed91ff53a601649/stardew-access/i18n/menu.en.ftl#L345-L367)
- New(en.ftl): `dynamic_tile-farm-lumber_pile` with english value `Lumber Pile`.
- Removed(static_tiles.en.ftl): `static_tile-farm-lumber_pile`.
- New(en.ftl): `inventory_util-special_items-name` with placeholder values at the moment.

### Tile Tracker Changes

- Bookseller's tile is now dynamically tracked.
- Detect Pierre's Booth tile in Luau festival.
- Detect lumber pile dynamically.

### Guides And Docs


### Misc

- Added pull request template
- ci: As opposed to `/fast-forward`, we can also now use `/fast-forward-force` to merge the PR without checking for `mergeable_state`.
- ci: Fix if condition failure in fast-forward.yml
