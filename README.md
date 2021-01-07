# robotsystemhw1
- リポジトリの概要
Raspberry PiでのLチカ
- 動作環境
Linux、Ubuntu20.04LTS
- 使用したもの
RaspberryPi4、ジャンパーワイヤ、赤色LED、ブレッドボード
- デモ動画のリンク
https://youtu.be/dB5733ZXMHQ
- インストール方法
git clone https://github.com/ShinnosukeTamai/robotsystemhw1.git
- 使用方法
LEDのアノードとgpio25を接続し、LEDのカソードをGNDに接続する。
make 、sudo insmod myled.ko　、chmod 666/dev/myled0 、の順に実行。
echo 0 > /dev/myled0で消灯
echo 1 > /dev/myled0で点灯
デモ動画では、echo 1 > /dev/myled0; sleep 3;echo 0 > /dev/myled0を実行し、3秒間点灯させた。
- ライセンス
GPL3.0LICENSE
- 引用
ryuichiueda
