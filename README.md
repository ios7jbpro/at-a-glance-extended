# Info
This is a complete open project to replicate the Google's At A Glance but with a better way with more options to customize. You can edit it however you want.
Just ask permission from me(Telegram: @ios7jbpro), and you can make your own releases based on this project. This is why I call it "open";).
# General Options

`::--Option:Monet(A12)--::`

This option is located under Globals>Global/mntflw.
How it runs is done by linking it to other buttons, by using;
```
$if(
gv(global/mntflw)=1,
(gv(monet)),
(gv(main/buttons/bgcolor)))$
```
This formula checks if global is on, and if it is, uses the color from Global>monet.
The "bgcolor" part is something else which will be explained also soon in a bit.

`::--Option:monet--::`

This option is located under Globals>monet.
The formula is;
```
$ce(si(wpcolor1), lum, 50)$
```
It's used to pull the wallpaper color.
