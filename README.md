# Info
This is a complete open project to replicate the Google's At A Glance but with a better way with more options to customize. You can edit it however you want.
Just ask permission from me(Telegram: @ios7jbpro), and you can make your own releases based on this project. This is why I call it "open";).
# General Options

`::--Option:Monet(A12)--::`

This option is located under Globals>Global/mntflw.
How it runs is done by linking it to other buttons, by using;
```
>$if(<
>gv(global/mntflw)=1,<
>(gv(monet)),<
(gv(main/buttons/bgcolor)))$
```
This formula checks if global is on, and if it is, uses the color from Global>monet.
The "bgcolor" part is something else which will be explained also soon in a bit.
The part between arrows indicate where it's used on.

`::--Option:monet--::`

This option is located under Globals>monet.
The formula is;
```
$ce(si(wpcolor1), lum, 50)$
```
It's used to pull the wallpaper color.

`::--Option:Color::`This option is located under Globals>Global/Color.
When this is set and Monet(A12) option is off, the UI will use this color instead for such stuff.
It's done by;
```
$if(
gv(global/mntflw)=1,
(gv(monet)),
>(gv(main/buttons/bgcolor)<))$
```
The part between arrows indicate where it's used on.

`::--Option:Shadow--::`

This option is located under Globals>Global/Shadow.
This option changes the amount of shadow/elevation that is displayed under the texts.
It's done by linking the shadow value on the texts to the global key.

`::--Option:LeftPadd--::`

This option is located under Globals>Global/LeftPadd.
This option is **NOT** changeable livetime from the widget. It changes the left side padding incase if there's anything on the left and needs to be adjusted.
The user can play with this from globals.

`::--Option:BtnRnd--::`

This option is located under Globals>Global/BtnRnd.
This option is **NOT** changeable livetime from the widget. It changes the roundness of the small buttons.
The user can play with this from globals.

`::--Option:Greetings--::`

This option is located under Globals>Global>Greetings.
This option enables the greetings text that shows from time to time.

`--::Options:grtntxt--::`

This option is located under Globals>Global/grtntxt.
This option is **NOT** changeable livetime from the widget. It changes the text that displays when Greetings key is on.
The user can play with this from globals.
