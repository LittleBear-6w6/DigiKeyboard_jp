# DigiKeyboard_jp
DigiKeyboardを日本語環境（日本語キーボード（106/109キー）下で記号（\ | . "  '等）を正しく出力するためのheaderファイルです。

# Requiremnet
 - Arduino IDE
 - Digistump AVR Boards by Digistump 1.6.7（Arduino IDEでDigistump開発を行うためのドライバー）

# Installation
 「DigiKeyboard_jp.h」と「scancode-ascii-table_jp.h」をArduinoにインストールしたDigistumpライブラリに追加する。

 1.Linux環境

```
   git clone https://github.com/LittleBear-6w6/DigiKeyboard_jp.git ~/work/
   mv DigiKeyboard_jp ~/.aruino15/packages/gidistump/hardware/avr/1.6.7/libraries/DigisparkKeyboard/
   mv scancod-ascii-table_jp.h ~/.aruino15/packages/gidistump/hardware/avr/1.6.7/libraries/DigisparkKeyboard/
```

 ※Windows環境にも同様のライブラリが格納されたフォルダがあると思いますのでそこへ入れてください。   
 　もしよろしければ、READMEに追記したいので情報をご教授ください！

# Usage
 スケッチソースで「DigiKeyboard.h」の代わりに「DigiKeyboard_jp.h」をインクルードする。

# License
  This source code is released under the GNU General Public License, see LICENSE.
  [digistump/DigisparkArduinoIntegration](https://github.com/digistump/DigisparkArduinoIntegration/tree/master/libraries/DigisparkKeyboard)で公開されているソースコードをもとに改変しているため、ライセンスについても参考もとに従う。

# Authors
 LittleBear-6w6

# References
 - digistump/DigisparkArduinoIntegration https://github.com/digistump/DigisparkArduinoIntegration/tree/master/libraries/DigisparkKeyboard
 - DigiKeyboardが日本語キーボード搭載PCで記号を正しく出力しない問題を解決する https://qiita.com/Toramin10/items/c1f63c51568ed00ed741
