[![Download: 1.0](https://img.shields.io/badge/Download-1.0-yellow?logo=docusign)](https://github.com/pervoj/jiconfont-font-awesome/releases/latest) [![Font Awesome version: 5.15.3](https://img.shields.io/badge/Font%20Awesome%20version-5.15.3-blue?logo=font-awesome)](https://github.com/FortAwesome/Font-Awesome/releases/tag/5.15.3) [![License: GPL 3.0](https://img.shields.io/badge/License-GPL%203.0-green)](https://github.com/pervoj/jiconfont-font-awesome/blob/master/LICENSE)

#  jIconFont – Font Awesome

*jIconFont – Font Awesome* is Java library, which expands the possibilities of the original library ([jIconFont - Font Awesome](http://jiconfont.github.io/fontawesome) by [Carlos Eduardo Leite de Andrade](https://github.com/caduandrade)) and uses latest versions of Font Awesome, and which can be used in Java Swing or JavaFX.

It aims to always be up to date with the latest version of Font Awesome.

For each Font Awesome icon style is there one class. There are three classes:
* `FontAwesomeSolid` – for [these](https://fontawesome.com/cheatsheet/free/solid) icons
* `FontAwesomeRegular` – for [these](https://fontawesome.com/cheatsheet/free/regular) icons
* `FontAwesomeBrands` – for [these](https://fontawesome.com/cheatsheet/free/brands) icons

## Usage

Each usage requires the jIconFont library: [https://search.maven.org/artifact/com.github.jiconfont/jiconfont](https://search.maven.org/artifact/com.github.jiconfont/jiconfont)

### Swing

For using in Swing you need to have jIconFont Swing library: [https://search.maven.org/artifact/com.github.jiconfont/jiconfont-swing](https://search.maven.org/artifact/com.github.jiconfont/jiconfont-swing)

Using in Swing is very simple. Here is example with solid style:

```java
IconFontSwing.register(FontAwesomeSolid.getIconFont());

Icon icon = IconFontSwing.buildIcon(FontAwesomeSolid.CHECK, 40, new Color(0, 150, 0));
JLabel label = new JLabel(icon);
```

### JavaFX

Using in JavaFX requires jIconFont JavaFX library: [https://search.maven.org/artifact/com.github.jiconfont/jiconfont-javafx](https://search.maven.org/artifact/com.github.jiconfont/jiconfont-javafx)

JavaFX usage is simple too:

```java
IconFontFX.register(FontAwesomeSolid.getIconFont());

IconNode iconNode = new IconNode(FontAwesomeSolid.CHECK);
iconNode.setIconSize(40);
iconNode.setFill(Color.DARKGREEN);
```

## How to get icon ID?

1. Go to this page: [https://fontawesome.com/icons](https://fontawesome.com/icons) and find icon, which you want to use.
2. Check if it is NOT pro icon.
3. Check what style the icon belongs to and select a class accordingly: `FontAwesomeSolid`, `FontAwesomeRegular` or `FontAwesomeBrands`.
4. Copy icon ID and use it as `FontAwesomeSolid.ICON_ID` (all in upper case and replace dashes with underscores).

![Font Awesome Catalog](https://user-images.githubusercontent.com/71781857/111660223-2533bf00-880e-11eb-91c8-e17764491612.png)
