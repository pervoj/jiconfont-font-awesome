#  jIconFont – Font Awesome

Package of latest Font Awesome fonts created for using with [jIconFont](http://jiconfont.github.io/).

For each Font Awesome icon style is there one class. There are three classes:
* `FontAwesomeSolid` – for [these](https://fontawesome.com/cheatsheet/free/solid) icons
* `FontAwesomeRegular` – for [these](https://fontawesome.com/cheatsheet/free/regular) icons
* `FontAwesomeBrands` – for [these](https://fontawesome.com/cheatsheet/free/brands) icons

## Usage

Each usage requires the jIconFont library: [http://jiconfont.github.io/](http://jiconfont.github.io/)

### Swing

Using in Swing is very simple. Here is example with solid style:

```java
IconFontSwing.register(FontAwesomeSolid.getIconFont());

Icon icon = IconFontSwing.buildIcon(FontAwesomeSolid.CHECK, 40, new Color(0, 150, 0));
JLabel label = new JLabel(icon);
```

### JavaFX

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