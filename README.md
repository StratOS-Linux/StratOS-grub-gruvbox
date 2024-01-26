<div align="center">
    <img src="/img/README-decorator.png" width=300/><br/>
    <h1> StratOS Grub Theme</h1>
</div>

## Preview

![preview](/img/low-res.jpeg)

## Compatibility

This should work on any Linux distribution that uses GRUB.

## Install

```bash
git clone https://github.com/StratOS-Linux/StratOS-grub.git
sudo mkdir -p /usr/share/grub/themes # just in case the directory doesn't exist
sudo cp -r StratOS-grub /usr/share/grub/themes/
sudo vim /etc/default/grub
```

Change `#GRUB_THEME=` to
`GRUB_THEME="/usr/share/grub/themes/StratOS-grub/theme.txt"`

```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

If all works correctly you should get this line in the out put:

```bash
Found theme: /usr/share/grub/themes/StratOS-grub/theme.txt
```

#### NOTE: For Fedora 37

When editing the file `/etc/default/grub`, you also have to comment the line `'GRUB_TERMINAL_OUTPUT="console"`

## Credit

- [Tartarus Grub](https://github.com/AllJavi/tartarus-grub)
- [grub2-gruvbox](https://git.fs.lmu.de/adnan/grub2-gruvbox) (for the install script)

## License

[MIT License](./LICENSE)
