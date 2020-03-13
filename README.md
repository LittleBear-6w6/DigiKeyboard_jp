# DigiKeyboard_jp
DigiKeyboardを日本語環境（日本語キーボード（106/109キー）下で記号（\ | . "  '等）を正しく出力するためのheaderファイルです。

This project is for the purpose of using DigiKeyboard on Japanese environment.   
We can input the identifier (\, | , " , ' etc) on Japanese environment by using this header files.

# Requiremnet
 - [Arduino IDE](https://www.arduino.cc/en/main/software)
 - Digistump AVR Boards by Digistump 1.6.7（Arduino IDEでDigistump開発を行うためのドライバー）
                                           (The driver for developing Digistump on Arduino IDE)
# Installation
 「DigiKeyboard_jp.h」と「scancode-ascii-table_jp.h」をArduinoにインストールしたDigistumpライブラリに追加する。

  Add DigiKeyBoard_jp.h and scancode-ascii-table_jp.h to Digistump library of Arduino.

 1.Linux環境 ( For Linux )

```
   git clone https://github.com/LittleBear-6w6/DigiKeyboard_jp.git ~/work/
   mv DigiKeyboard_jp ~/.aruino15/packages/digistump/hardware/avr/1.6.7/libraries/DigisparkKeyboard/
   mv scancod-ascii-table_jp.h ~/.aruino15/packages/digistump/hardware/avr/1.6.7/libraries/DigisparkKeyboard/
```

 ※Windows環境にも同様のライブラリが格納されたフォルダがあると思いますのでそこへ入れてください。   
 　もしよろしければ、READMEに追記したいので情報をご教授ください！

# Usage
 スケッチソースで「DigiKeyboard.h」の代わりに「DigiKeyboard_jp.h」をインクルードする。
 
 Include DigiKeyboard_jp.h instead of DigiKeyboard.h when we write sketch code.

# License
  This source code is released under the GNU General Public License, see LICENSE.<br>
  [digistump/DigisparkArduinoIntegration](https://github.com/digistump/DigisparkArduinoIntegration/tree/master/libraries/DigisparkKeyboard)で公開されているソースコードをもとに改変しているため、ライセンスについても参考もとに従う。

# Authors
 LittleBear-6w6

# References
 - digistump/DigisparkArduinoIntegration https://github.com/digistump/DigisparkArduinoIntegration/tree/master/libraries/DigisparkKeyboard
 - DigiKeyboardが日本語キーボード搭載PCで記号を正しく出力しない問題を解決する https://qiita.com/Toramin10/items/c1f63c51568ed00ed741

# Change log
 - 2020/02/23   First Commit.
 - 2020/03/13   Modify becuase we cann't input the identifier of parentheses and astarisk.
