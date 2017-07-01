# Known intermittent failures

This file is parsed when running automated tests on our CI.

Known failures are shown in logs, but status will be green unless it is an uknown failure.
These browser level tests are prone to intermittent failures and without ignoring known failures,
it makes it very hard to know what is safe and what is not safe to merge from PRs.

Parsing of this file simply looks for lines that start with "- " which indicates a known test failure.

## lint

There are no acceptable lint failures.

## unit

There are no acceptable unit test failures.

## about

- Advanced payment panel tests can backup wallet to file
- Advanced payment panel tests can recover wallet from file
- Advanced payment panel tests shows an error popover if a recovery key is not a UUID
- Advanced payment panel tests shows an error popover if both recovery keys are missing
- Advanced payment panel tests shows an error popover if one recovery key is missing
- Advanced payment panel tests shows an error popover if the file is empty
- Ledger table 2 publishers check if all sites are on the unpinned by default
- Ledger table 2 publishers pin publisher and change percentage
- Ledger table 4 publishers check if all sites are on the unpinned list
- Ledger table 4 publishers pin 3 publishers
- Ledger table 4 publishers pin 3 publishers custom value and check unpinned value
- Regular payment panel tests can setup payments "before each" hook for "shows welcome page"

## app

- MessageBox component tests alert when opening a new tab (while alert is showing) lets you use the back button
- MessageBox component tests alert when opening a new tab (while alert is showing) lets you use the forward button

## bookmark-components

## bravery-components

- Bravery Panel Adblock stats iframe tests detects blocked elements in iframe
- Bravery Panel Adblock stats iframe tests detects blocked elements in iframe in private tab
- Bravery Panel Adblock stats without iframe tests block device enumeration
- Bravery Panel Adblock stats without iframe tests detects adblock resources in private tab
- Bravery Panel Adblock stats without iframe tests downloads and detects regional adblock resources in private tab
- Bravery Panel Tracking Protection stats detects blocked elements
- Clear Browsing Panel with saved state values saves the history switch state
- noscript info can allow scripts on a file:// URL without allowing all scripts
- noscript info can selectively allow scripts

## contents

## misc-components

- Syncing and clearing data prevents it from syncing "before all" hook
- Syncing bookmarks "before all" hook
- Syncing bookmarks from an existing profile "before all" hook
- Syncing then turning it off stops syncing "before all" hook
- findBar typing while another frame is loading

## navbar-components

- navigationBar tests navigation tabnapping updates the location in the navbar when changed by the opener
- navigator component tests lion badge is grayed out if shield is disabled
- urlBar tests autocomplete "before each" hook for "clears the selection"
- urlBar tests keeps url text separate from suffix text changes only the selection

## tab-components

- tab tests tab transfer can detach into new windows
