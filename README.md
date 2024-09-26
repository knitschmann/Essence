# Essence - One Liner with minimal URL Bar Edition

## Short description

Essence is a compact, beautiful, and minimalistic one-liner theme for the Firefox web browser. The main goal was to minify a toolbar, so more content would be displayed in the browser.

Firefox Containers feature a colorful glow on each tab.

## Screenshots

![Tabs on the Right](https://github.com/knitschmann/Essence/blob/753219e21b746418f88ace1d5520ad0f07d1a784/tabs-right.jpg)
![Tabs on the Left](https://github.com/knitschmann/Essence/blob/753219e21b746418f88ace1d5520ad0f07d1a784/tabs-left.jpg)

## Installation

1. Open Firefox and navigate to `about:config`.
2. Click on "Accept the Risk and Continue" to proceed.
3. Double-click on `toolkit.legacyUserProfileCustomizations.stylesheets` to enable it if it's not already enabled.
7. Open the root directory of your profile.
8. Create a folder called `chrome` if it doesn't already exist.
9. Copy the `userChrome.css` file from the cloned repository into the `chrome` folder.
10. To align all UI buttons such as navigation, extensions and bookmarks, set the following in your user.js (depends on your specific addon installation):

```
user_pref("browser.uiCustomization.state", "{\"placements\":{\"widget-overflow-fixed-list\":[],\"unified-extensions-area\":[\"sponsorblocker_ajay_app-browser-action\",\"_testpilot-containers-browser-action\",\"admin_2fas_com-browser-action\"],\"nav-bar\":[\"urlbar-container\",\"back-button\",\"stop-reload-button\",\"customizableui-special-spring1\",\"customizableui-special-spring2\",\"reset-pbm-toolbar-button\",\"unified-extensions-button\",\"downloads-button\"],\"toolbar-menubar\":[\"menubar-items\"],\"TabsToolbar\":[\"tabbrowser-tabs\",\"new-tab-button\",\"personal-bookmarks\",\"bookmarks-menu-button\",\"ublock0_raymondhill_net-browser-action\",\"_446900e4-71c2-419f-a6a7-df9c091e268b_-browser-action\",\"alltabs-button\"],\"PersonalToolbar\":[\"import-button\"],\"vertical-tabs\":[]},\"seen\":[\"save-to-pocket-button\",\"reset-pbm-toolbar-button\",\"profiler-button\",\"developer-button\",\"_446900e4-71c2-419f-a6a7-df9c091e268b_-browser-action\",\"ublock0_raymondhill_net-browser-action\",\"sponsorblocker_ajay_app-browser-action\",\"_testpilot-containers-browser-action\",\"admin_2fas_com-browser-action\"],\"dirtyAreaCache\":[\"nav-bar\",\"vertical-tabs\",\"PersonalToolbar\",\"toolbar-menubar\",\"TabsToolbar\",\"unified-extensions-area\"],\"currentVersion\":20,\"newElementCount\":12}");
```


(for the version with tabs on the left and url bar on the right, use:)
```
user_pref("browser.uiCustomization.state", "{\"placements\":{\"widget-overflow-fixed-list\":[],\"unified-extensions-area\":[\"sponsorblocker_ajay_app-browser-action\",\"_testpilot-containers-browser-action\",\"admin_2fas_com-browser-action\"],

	\"nav-bar\":[\"unified-extensions-button\",\"downloads-button\",\"back-button\",\"forward-button\",\"stop-reload-button\",\"reset-pbm-toolbar-button\",\"urlbar-container\"],

	\"toolbar-menubar\":[\"menubar-items\"],\"TabsToolbar\":[\"tabbrowser-tabs\",\"new-tab-button\",\"personal-bookmarks\",\"bookmarks-menu-button\",\"ublock0_raymondhill_net-browser-action\",\"_446900e4-71c2-419f-a6a7-df9c091e268b_-browser-action\",\"alltabs-button\"],\"vertical-tabs\":[],


	\"PersonalToolbar\":[\"import-button\"]},\"seen\":[\"save-to-pocket-button\",\"reset-pbm-toolbar-button\",\"profiler-button\",\"developer-button\",\"_446900e4-71c2-419f-a6a7-df9c091e268b_-browser-action\",\"ublock0_raymondhill_net-browser-action\",\"sponsorblocker_ajay_app-browser-action\",\"_testpilot-containers-browser-action\",\"admin_2fas_com-browser-action\"],\"dirtyAreaCache\":[\"nav-bar\",\"vertical-tabs\",

	\"PersonalToolbar\",


	\"toolbar-menubar\",\"TabsToolbar\",\"unified-extensions-area\"],\"currentVersion\":20,\"newElementCount\":20}");
```

## Credits

This repository is a fork of [Bali10050/FirefoxCSS](https://github.com/Bali10050/FirefoxCSS), with various modifications, removals, and additions. Some code snippets were also sourced from the [denizjcan/Firefox-Safari-15-Theme](https://github.com/denizjcan/Firefox-Safari-15-Theme) repository. The icons used in the theme are taken from Google Material Symbols.

The style of tabs left with the url bar on theright is based on: https://github.com/MrOtherGuy/firefox-csshacks/blob/master/chrome/navbar_tabs_oneliner_tabs_on_left.css
