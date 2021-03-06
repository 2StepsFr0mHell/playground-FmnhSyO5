# Release notes

The CodinGame SDK is regularly updated and improved. This document lets you know what changed in the latest releases.

## 3.1.0

### 🎁 New feature

- A frame is created even if no players have been executed at the end of each gameTurn.

### 🐞 Bug fix

- Fixed an issue with sprites

## 3.0.0
*January 11, 2019*

### 🎁 New features

- [BitmapText](playground/graphics/graphics-text.md#BitmapText) has been added.
- [Text](playground/graphics/graphics-text.md#Text) can be bold.
- Shapes now have a blendmode property.

### 🐞 Bug fixes

- 💥 _Breaking change_ Renamed SpriteSheetLoader to SpriteSheetSplitter.
- Subfolders of the assets folder work on Windows now.
- Frame zero now has a duration of zero.
- The [SpriteSheetSplitter](playground/graphics/graphics-4-spritesheets.md#SpriteSheetSplitter) doesn't reload the sprite sheet if it's already in the TextureCache.
- The local player now uses the parameters stored in the LocalStorage.
- Removed the max turn warning, since it's replaced by a limit of alloted time.
- Better process cleanup.
- Fixed security issue (ZipSlip bug).
- Fixed the minimum max time alloted to players (now it really is 50ms).


## 2.15
*November 29, 2018*

### 🐞 Bug fixes

- Frame zero is not animated anymore.
- Less spammy warnings.

## 2.14
*October 30, 2018*

### 🎁 New features

- Limited the max total alloted time to the players to 25s.
- SpriteAnimation now a has reworked API and a pause function.

### 🐞 Bug fixes

- Better error handling.
- Reworked the commit system, fixing some big issues and reducing data usage.

## 2.11
*September 14, 2018*

### 🐞 Bug fixes

- Fixed BufferedGroup performance issues.
- Better handling of modules errors.

## 2.9
*August 21, 2018*

### 🎁 New feature

- Local test page design now matches the website one

## 2.8
*August 9, 2018*

### 🐞 Bug fixes

- Reworked the Test case API.
- Fixed some WEBGL memory leaks.

## 2.7
*August 1, 2018*

### 🐞 Bug fixes

- Handling of the absence of a logo in the demo.
- Limiting the size of the game summary.

## 2.5
*July 6, 2018*

### 🎁 New feature
 - Game Params are now displayed in the local test page.

## 2.4
*June 25, 2018*

### 🎁 New feature

- [Buffered Groups](playground/graphics/graphics-6-advanced.md#buffered-groups) have been added.

### 🐞 Bug fixes

- Test cases can now handle several lines as input.
- The configuration verification does not check the presence of `welcome_en.html` in the first league anymore. It also concerns games with no league system.

## 2.3
*June 8, 2018*

### 🐞 Bug fixes

- The `BindException` thrown when running a new instance of the game when the server is already on use has been caught. It now logs a warning.
- A bug would prevent you from exporting a game that was too heavy. It is now fixed.

## 2.2
*June 4, 2018*

### 🐞 Bug fixes

- Solo games agents not having colors would produce an error once uploaded on CodinGame. A default color has been added.
- A regression would prevent the configuration form from being displayed. This feature is back.

## 2.1
*June 1, 2018*

### Bug fix

- The Graphic Entity Module would stop displaying the last frame of a replay. This is now fixed.

## 2.0
*June 1, 2018*

### 🎁 New features

- [Solo](playground/getting-started/tutorial-3-solo.md) and [Optimization](playground/getting-started/tutorial-4-opti.md) games have been added.
    - Implementation of Multiplayer and Solo classes extending from formerly used `AbstractPlayer`, `GameManager` and `GameRunner`. These features are *not* backward compatible.
    - [Test cases](playground/core-concepts/core-4-configuration.md#test-case-file) have been added.
    - The configuration verification has been updated to match the new constraints.
    - The form to set up basic configurations when exporting the game has been updated. It now handles the different type of games and specific settings for each of them.

## 1.37 and older versions

These versions are not handled anymore and your game will not work if you upload it on CodinGame. If you are still using this version, it is strongly recommended to update your project to the latest release.