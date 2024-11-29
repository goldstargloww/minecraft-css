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
| black | <img src="https://sheep.greysdawn.com/color/000000?text=%20" width="32"> | #000
| dark_blue | <img src="https://sheep.greysdawn.com/color/0000aa?text=%20" width="32"> | #00A
| dark_green | <img src="https://sheep.greysdawn.com/color/00aa00?text=%20" width="32"> | #0A0
| dark_aqua | <img src="https://sheep.greysdawn.com/color/00aaaa?text=%20" width="32"> | #0AA
| dark_red | <img src="https://sheep.greysdawn.com/color/aa0000?text=%20" width="32"> | #A00
| dark_purple | <img src="https://sheep.greysdawn.com/color/aa00aa?text=%20" width="32"> | #A0A
| gold | <img src="https://sheep.greysdawn.com/color/ffaa00?text=%20" width="32"> | #FA0
| gray | <img src="https://sheep.greysdawn.com/color/aaaaaa?text=%20" width="32"> | #AAA
| dark_gray | <img src="https://sheep.greysdawn.com/color/555555?text=%20" width="32"> | #555
| blue | <img src="https://sheep.greysdawn.com/color/5555ff?text=%20" width="32"> | #55F
| green | <img src="https://sheep.greysdawn.com/color/55ff55?text=%20" width="32"> | #5F5
| aqua | <img src="https://sheep.greysdawn.com/color/55ffff?text=%20" width="32"> | #5FF
| red | <img src="https://sheep.greysdawn.com/color/ff5555?text=%20" width="32"> | #F55
| light_purple | <img src="https://sheep.greysdawn.com/color/ff55ff?text=%20" width="32"> | #F5F
| yellow | <img src="https://sheep.greysdawn.com/color/ffff55?text=%20" width="32"> | #FF5
| white | <img src="https://sheep.greysdawn.com/color/ffffff?text=%20" width="32"> | #FFF
