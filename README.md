# PvPoke.com to Poracle
A simple repo that convert the [rankings of PvPoke.com](https://pvpoke.com/rankings/) to [Poracle](https://github.com/KartulUdus/PoracleJS) commands or Pokémon aliases. 
All of those commands/aliases are updated automatically on the CI.

## Pokemon aliases
Add those aliases to the file `config/pokemonAlias.json`. 

<!-- aliases-start -->
```json
{
  "top30Great": [
    379, 618, 560, 308, 260, 709, 411, 164, 279, 334, 108, 472, 171, 18, 302,
    832, 68, 630, 226, 799, 288, 38, 340, 660, 784, 377, 197, 202, 699, 386,
    460, 748, 488, 149
  ],
  "top30Ultra": [
    379, 18, 487, 377, 472, 709, 638, 260, 488, 208, 640, 799, 794, 862, 6, 699,
    788, 618, 560, 365, 38, 378, 460, 832, 630, 646, 663, 149, 279, 197, 241,
    186, 144, 784, 463, 9, 386, 589, 226, 154, 145, 131, 164
  ],
  "top30Master": [
    383, 487, 249, 646, 791, 149, 648, 150, 888, 717, 644, 671, 130, 716, 643,
    484, 473, 893, 483, 250, 382, 809, 143, 645, 649, 260, 635, 376, 445, 794,
    901, 381, 889, 146, 145, 151, 639, 640, 713, 784, 638, 530, 377
  ]
}
```
<!-- aliases-end -->

After restarting Poracle, you can easily track those Pokémon like this:
```shell
!track top30Great great1
!track top30Ultra ultra1
```

## Commands
Poracle is able to process track commands in bulk, so you can easily copy and paste those commands to track every Pokémon. 
Also, since legendaries are not always available in the wild, they aren't counted when making the top 30, but still added to the list just in case.

### Rank 1 of the top 30 Pokémon in great league ranking
<!-- top30great-start -->
```
!track great1 379 618 560 308 260 709 411 164 279 334 108 472 171 18 302 832 68 630 226 799 288 38 340 660 784 377 197 202 699 386 460 748 488 149
```
<!-- top30great-end -->

### Rank 1 of the top 30 Pokémon in ultra league ranking
<!-- top30ultra-start -->
```
!track ultra1 379 18 487 377 472 709 638 260 488 208 640 799 794 862 6 699 788 618 560 365 38 378 460 832 630 646 663 149 279 197 241 186 144 784 463 9 386 589 226 154 145 131 164
```
<!-- top30ultra-end -->
