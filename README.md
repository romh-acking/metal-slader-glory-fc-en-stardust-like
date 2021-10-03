[//]: <> (This readme is in the markdown format. Please preview in a markdown parser.)

# Metal Slader Glory FC: Translation (Stardust-like Edition)

## About
This repository contains source code for patches and tools to compile an English translation of Metal Slader for the Famicom.

This is a fork of the [metal-slader-glory-fc-en-8x8](https://github.com/romh-acking/metal-slader-glory-fc-en-8x8) repository. If you're a fan of the Stardust Crusaders translation, then this is the project for you. The text speed is slowed down, just like that translation, and uses the font from it.

This fork was created because it's a somewhat common request. I think [metal-slader-glory-fc-en](https://github.com/romh-acking/metal-slader-glory-fc-en) is the definitive version, so I would suggest playing that one instead.

## Changes
* Text speed decreased
* Cutscene timing changed by shortening text or by adjusting control codes.
* Some text overflow issues fixed due to the removal of squishy text. There's very likely more.
* Font reverted to the one from Stardust Crusader translation
	* The robotic font is from the Jesus translation. It could be better honestly.

## Issues
* This patch removes the squishy text tiles. While the autolinebreaking will adjust the linebreaks accordingly, there's probably some text overflow issues. This may be due to portraits being present that the inserter isn't expecting. Add `\LineWidthPortraitShowing/` at the beginning of lines to fix this. This also may be because there's not enough room for menu options. For this, you'll have to shorten them.
* The screen tweak screen and game over screen are garbled because they weren't adjusted to accomodate the new font.

## Licensing
If you're using this repository as a base, please remember this project is licensed under the GLP3 license. The license notice must be preserved and the project *must* be open source.