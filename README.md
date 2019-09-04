# polybar-cryptocurrency

![pcrypto](https://user-images.githubusercontent.com/21110159/64199525-30750300-ce93-11e9-812b-0eaf94494b1f.png)

A polybar script much like [polybar-crypto](https://github.com/willHol/polybar-crypto).
It's a great script, but: 
* I dislike messing with configuration files for small scripts
* I feel as if changing what the module displays should be quick
* [Coinranking's API](https://docs.coinranking.com/public) is much better than CMC, in my opinion (currency symbols)
* [Guarda's icons](https://github.com/guardaco/crypto-icons) are recent and look really nice, and it's fun to be able to fetch them quickly

## Setup
```
git clone https://github.com/SplendidX/polybar-cryptocurrency.git

cd polybar-cryptocurrency && ./setup.sh
```
__or__ copy coins.otf to ~/.fonts, and coins.svg & pcrypto.py to ~/.config/polybar

### Module
Add to your polybar config:
```
[bar/my-left]
modules-right = crypto

[module/crypto]
type = custom/script
exec = ~/.config/polybar/pcrypto.py --base USD --coins btc eth link ltc xrp xmr
interval = 60
<<<<<<< HEAD
```

### Icons
Icons are fetched from coins.svg, if you'd like to use your own icon for a specific coin, just replace the unicode with the icon
```
:btc
```

more options in `pcrypto.py -h`
=======

font-0 = "coins:style=Regular;0"
```
more options in `pcrypto.py -h`
>>>>>>> 1a74e57275194d7dafd1df7df0b408187b2ac695
