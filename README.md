![Demo@2x](https://user-images.githubusercontent.com/2870726/152635538-87dcfe70-bcf8-421d-92a5-23e68a408db7.png)


# macOS Native-looking Translucent Tabbar for Firefox 

Replaces default Firefox black-and-white theme with a more native-looking light/dark compatible translucent tabbar.
You need to set your theme to "Default" for this tweak to properly work. Works best if you set your system appearance to "Auto" (changing light/dark automatically), then Firefox will follow the OS settings for color scheme.

**⚠️ Note: this tweak will only work on macOS versions of Firefox.**

## Firefox 127 and newer

1. Go to `about:config` on your URL bar, search for below two values set them to `true` (double-click the value to change).
   - `widget.macos.titlebar-blend-mode.behind-window`
   - `browser.theme.macos.native-theme`
2. Give Firefox a restart and your tab bar should turn translucent.

(Thanks @la3rence for the tip [#12](https://github.com/zvuc/firefox-macos-native-tabbar/issues/12))

## Firefox 126 and older
1. Go to `about:support` in URL bar. Look for "Profile Folder" then click "Show In Finder" button to open the profile folder.
2. Create a new folder named `chrome`.
3. Create a new blank file named `userChrome.css`
4. Copy-and-paste the code included in the `macos-native-tabbar.css` file.
5. Go to `about:config` on your URL bar, search for `toolkit.legacyUserProfileCustomizations.stylesheets` and make sure it's set to `true` (double-click the value to change).
6. Starting from Firefox 126 and above, you also need set `widget.macos.titlebar-blend-mode.behind-window` as `true`. (Thanks @emilio! [#11](https://github.com/zvuc/firefox-macos-native-tabbar/issues/11))
7. Give Firefox a restart and your tab bar should turn translucent.

For a more thorough guide on using userChrome.css, please refer to this wonderful guide at [userchrome.org](https://www.userchrome.org/how-create-userchrome-css.html).

## See also
[Firefox Sliding Bookmarks Bar](https://github.com/zvuc/firefox-sliding-bookmarks-bar/) - Tuck in the bookmarks bar under toolbar to make it slide out only on mouse hover. Makes your firefox cleaner & minimal!

## License
MIT License
