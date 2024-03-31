# minecraft css

hey! i got frustrated with there being no good ways of recreating minecraft visuals using something like css, and it eventually frustrated me enough that i ended up doing it myself.

i recreated the minecraft seven font (for the most part, there's *definitely* a few errors) and spent some time implementing various text-based visuals into css. currently, it includes all 16 color codes, text shadows, bold / italic / strikethrough / underlined text, titles, subtitles, and chat.

you can see how it looks [here](https://goldstargloww.github.io/minecraft-css/)!

feel free to use this! i made it because nobody had already. just grab the `minecraft.css` file as well as the fonts and you're all set :>

## what's going on with the colors?

yeah okay fair it looks complicated

basically, the way minecraft colors work is that there's 4 values for different levels of each RGB channel: `0`, `85`, `170`, and `255`. every default color is some combination of these numbers. the color of a color's shadow is calculated by dividing the value of each channel by 4. 

so gold is `rgb(255, 170, 0)`, and its shadow is `rgb(255/4, 170/4, 0/4)`, or `rgb(64, 42, 0)`.

### why are they called that?

because that's how minecraft does it

| name | color | hex
| -- | -- | --
| black | <img src="https://color.petalss.me/000000.png" width="32"> | #000
| dark_blue | <img src="https://color.petalss.me/0000AA.png" width="32"> | #00A
| dark_green | <img src="https://color.petalss.me/00AA00.png" width="32"> | #0A0
| dark_aqua | <img src="https://color.petalss.me/00AAAA.png" width="32"> | #0AA
| dark_red | <img src="https://color.petalss.me/AA0000.png" width="32"> | #A00
| dark_purple | <img src="https://color.petalss.me/AA00AA.png" width="32"> | #A0A
| gold | <img src="https://color.petalss.me/FFAA00.png" width="32"> | #FA0
| gray | <img src="https://color.petalss.me/AAAAAA.png" width="32"> | #AAA
| dark_gray | <img src="https://color.petalss.me/555555.png" width="32"> | #555
| blue | <img src="https://color.petalss.me/5555FF.png" width="32"> | #55F
| green | <img src="https://color.petalss.me/55FF55.png" width="32"> | #5F5
| aqua | <img src="https://color.petalss.me/55FFFF.png" width="32"> | #5FF
| red | <img src="https://color.petalss.me/FF5555.png" width="32"> | #F55
| light_purple | <img src="https://color.petalss.me/FF55FF.png" width="32"> | #F5F
| yellow | <img src="https://color.petalss.me/FFFF55.png" width="32"> | #FF5
| white | <img src="https://color.petalss.me/FFFFFF.png" width="32"> | #FFF