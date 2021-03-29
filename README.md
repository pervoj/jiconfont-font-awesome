[![Download: 1.0.2](https://img.shields.io/badge/Download-1.0.2-yellow?logo=docusign)](https://search.maven.org/artifact/com.github.pervoj/jiconfont-font-awesome/1.0.2/jar) [![Font Awesome version: 5.15.3](https://img.shields.io/badge/Font%20Awesome%20version-5.15.3-blue?logo=font-awesome)](https://github.com/FortAwesome/Font-Awesome/releases/tag/5.15.3) [![License: GPL 3.0](https://img.shields.io/badge/License-GPL%203.0-green)](https://github.com/pervoj/jiconfont-font-awesome/blob/master/LICENSE)

#  jIconFont – Font Awesome

*jIconFont – Font Awesome* is Java library, which expands the possibilities of the original library ([jIconFont - Font Awesome](http://jiconfont.github.io/fontawesome) by [Carlos Eduardo Leite de Andrade](https://github.com/caduandrade)) and uses latest versions of Font Awesome, and which can be used in Java Swing or JavaFX.

It aims to always be up to date with the latest version of Font Awesome.

For each Font Awesome icon style is there one class. There are three classes:
* `FontAwesomeSolid` – for [these](https://fontawesome.com/cheatsheet/free/solid) icons
* `FontAwesomeRegular` – for [these](https://fontawesome.com/cheatsheet/free/regular) icons
* `FontAwesomeBrands` – for [these](https://fontawesome.com/cheatsheet/free/brands) icons

## How to get?

You can download this library from [GitHub repository releases](https://github.com/pervoj/jiconfont-font-awesome/releases), [Maven Central repository](https://search.maven.org/artifact/com.github.pervoj/jiconfont-font-awesome), or you can use it as Maven dependency:

```xml
<dependency>
    <groupId>com.github.pervoj</groupId>
    <artifactId>jiconfont-font-awesome</artifactId>
    <version>1.0.2</version>
</dependency>
```

## Usage

Each usage requires the [jIconFont library](https://search.maven.org/artifact/com.github.jiconfont/jiconfont).

If you are using this library as Maven dependency, this requirement will be attached automatically.

### Swing

Using in Swing requires [jIconFont - Swing](https://search.maven.org/artifact/com.github.jiconfont/jiconfont-swing) dependency.

How it use? It's simple. Here is example with solid style:

```java
IconFontSwing.register(FontAwesomeSolid.getIconFont());

Icon icon = IconFontSwing.buildIcon(FontAwesomeSolid.CHECK, 40, new Color(0, 150, 0));
JLabel label = new JLabel(icon);
```

### JavaFX

Using in JavaFX requires [jIconFont - JavaFX](https://search.maven.org/artifact/com.github.jiconfont/jiconfont-javafx) dependency.

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
