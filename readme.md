# setup
gh repo clone saitotqr/qmk_firmware
git submodule update --init --recursive


# build
make crkbd/rev1/common:via
make crkbd/rev1/common:via:avrdude

or

qmk compile -kb crkbd/rev1 -km default

# helix memo
helix/rev3-5rows
qmk修正箇所とコンパイル方法
```
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   keyboards/helix/rev3_5rows/keymaps/five_rows/config.h
        modified:   keyboards/helix/rev3_5rows/keymaps/five_rows/keymap.c

~/qmk_firmware via :snake: v2.7.16 on  master [$+⇡] 15:14:01 383ms
❯ qmk compile -kb helix/rev3_5rows -km five_rows

```
keymap.c は古いVerを置いておく
config.h はロストした
