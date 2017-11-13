`ivy-window-configuration` offers a more robust solution to managing [`window-configurations`](https://www.gnu.org/software/emacs/manual/html_node/elisp/Window-Configurations.html) than [registers](https://www.gnu.org/software/emacs/manual/html_node/emacs/Configuration-Registers.html#Configuration-Registers).

![](https://asimpson.github.io/ivy-window-configuration/images/ivy-view.png)

I was inspired by [`ivy-switch-view`](https://github.com/abo-abo/swiper/blob/301139d142cb091328453f0fa2bd067d17f943f7/ivy.el#L3614). However `ivy-switch-view` has a different design as stated in [this issue thread]( https://github.com/abo-abo/swiper/pull/587#issuecomment-233167085). Using `window-configuration`s means that positions and dimensions of buffers are restored perfectly. In practice this feels much like `tmux`'s "zoom" feature which lets you toggle away every pane but the selected one and change things back.


`ivy-window-configuration` comes with a [hydra](https://github.com/abo-abo/hydra): `ivy-window-configuration--hydra/body` which exposes all the functionality in a single screen.
`ivy-window-configuration` also works via a standard ivy/counsel interface with deletes bound to `M-o d` and `M-o D` respectively.

![](https://asimpson.github.io/ivy-window-configuration/images/ivy-options.png)

![](https://asimpson.github.io/ivy-window-configuration/images/ivy-hydra.png)
