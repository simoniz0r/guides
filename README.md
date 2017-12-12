# Customizing LXQt with Openbox

Required packages: lxqt (metapackage that provides entire LXQt DE which should include Openbox), lxappearance (used for setting the GTK theme, icons, cursors, and fonts), qt5-style-plugins (provides the option to use GTK theme for LXQt's widget setting), and compton (compton-conf can also be installed for GUI config).  You can also install obconf-qt for a nicer looking Openbox GUI config.

![screenshot](/screenshots/full-desktop.png)

![screenshot2](/screenshots/full-desktop2.png)

# LXQt's Appearance settings

Open up the `LXQt Configuration Center` app and then open up `Appearance`.

![lxqt-config](/screenshots/lxqt-config.png)

In LXQt's Appearance settings, select the `gtk2` option for the Widget Style.  This will allow us to use any GTK theme that we want to theme pretty much all of the applications running on our system.

![widget-style](/screenshots/widget-style.png)

Next we'll go to the Icons Theme secton in `Appearance`.  You can choose whatever icon theme you like.  I am using [Papirus icons + Breeze action icons ](https://www.opendesktop.org/p/1192944/) (the dark version).  The icons chosen here will only apply to Qt applications since we have `lxappearance` installed, but we'll take care of that later.

![lxqt-icons.png](/screenshots/lxqt-icons.png)

In the LXQt Theme section of `Appearance`, we want to make sure to select the `System` option so that the color from our GTK theme will be used for LXQt's panel, menus, etc.

![lxqt-theme.png](/screenshots/lxqt-theme.png)

In the Fonts section of `Appearance`, you can use whatever fonts you like.  I am using Noto Sans size 11.  The antialiasing, hinting, and DPI settings are also found here.

![lxqt-font](/screenshots/lxqt-font.png)

You can also select whatever Cursors in `Appearance`.  I am using the [Polar Cursor Theme](https://www.opendesktop.org/p/999968/).

![lxqt-cursor](/screenshots/lxqt-cursor.png)

# Customize Look and Feel (lxappearance)

Open `Customize Look and Feel` in your menu to open `lxappearance`.  In the Widget tab, we'll select our GTK theme.  I am using [Breeze-gtk](https://www.opendesktop.org/p/1197982/) (dark version; included in Breeze-gtk download).  This theme will apply to pretty much all applications that we run on our system.

On the same tab just below the preview of the selected GTK theme is the font setting for GTK apps.  We'll want to make sure we used the same font as above.

![gtk-widget](/screenshots/gtk-widget.png)

The next tab in `lxappearance` is the Color tab, but this only applies if you are running LXDE, so we will skip this tab and move to the Icon Theme.  We'll want to make sure to select the same icon theme that we used above.

![gtk-icons](/screenshots/gtk-icons.png)

Once again in the Mouse Cursor tab of `lxappearance`, we'll want to make sure to select the same cursors as above.

![gtk-cursor](/screenshots/gtk-cursor.png)

In the Window Border tab of `lxappearance`, we will set the theme that Openbox uses for its window borders.  I am using a customized version of Minstral-Thin-Dark that is included in the `.themes` directory of this repo.

![ob-border](/screenshots/ob-border.png)

The final tab that we should cover here is the Font tab of `lxappearance`.  This contains the antialiasing and hinting settings for GTK fonts.  We'll want to make sure to use the same settings we used above.

![gtk-font-aa](/screenshots/gtk-font-aa.png)

# More to come

This is the end for now.  I have included by Openbox and LXQt settings in the `.config` directory of this repo.  I'll go into more detail on how to change those settings when I find time to finish this :)
