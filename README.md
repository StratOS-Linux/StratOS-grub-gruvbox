<div align="center">
    <img src="/img/README-decorator.png" width=300/><br/>
    <h1> LUGOS Grub Theme</h1>
</div>

## Preview

![preview](/img/low-res.png)

## Compatibility

This should work on any Linux distribution that uses GRUB, but I have only tested it on EndeavourOS and Kali

## Install

```bash
git clone https://github.com/slipstream8125/LUGOS-grub.git
cd LUGOS-grub
sudo cp LUGOS-grub -r /usr/share/grub/themes/
sudo vim /etc/default/grub
```

Change `#GRUB_THEME=` to
`GRUB_THEME="/usr/share/grub/themes/LUGOS-grub/theme.txt"`

```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

If all works correctly you should get this line in the out put:

```bash
Found theme: /usr/share/grub/themes/LUGOS-grub/theme.txt
```

#### NOTE: For Fedora 37

When editing the file `/etc/default/grub`, you also have to comment the line `'GRUB_TERMINAL_OUTPUT="console"`

## Credit

- [Cute Ghost profile](https://www.flaticon.com/free-icon/ghost_1150381?term=ghost&page=1&position=52&page=1&position=52&related_id=1150381&origin=style)
- [Dracula Grub](https://draculatheme.com/grub)
- [Tokyo Night Grub](https://github.com/mino29/tokyo-night-grub)
- [Tartarus Grub](https://github.com/AllJavi/tartarus-grub)

## License

[MIT License](./LICENSE)
