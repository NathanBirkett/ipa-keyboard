# ipa-keyboard
![](https://github.com/NathanBirkett/ipa-keyboard/blob/main/layout.png)

## Description
This is an ahk file that maps every standard IPA character onto a keyboard. Because of how many symbols there are, this requires overriding many more keys than a usual keyboard layout like the right control, alt, and shift keys. It also makes use of the numpad and keys like Insert, Scroll Lock, Page Up, etc. For keyboards that dont have a numpad, I have mapped some key combinations with Alt to the numpad. Note that keyboard shortcuts like Ctrl+c and Ctrl+z still work. Most keyboards have special combinations to input keys like Insert, Scroll Lock, Page Up, etc. if they don't have buttons for them, so this might take some research for your specific computer. If not, feel free to edit the script directly, the format is pretty self explanatory.
![](https://github.com/NathanBirkett/ipa-keyboard/blob/main/layout_diagram.png)

## Layout
![](https://github.com/NathanBirkett/ipa-keyboard/blob/main/numpad_sub_diagram.png)
In general left to right goes back in the mouth, like in the IPA chart.
- Nasals (red): Pressing shift gives some common auxiliary symbols
- Plosives (green): By default they are unvoiced, and pressing shift will voice them.
- Fricatives (blue): As with plosives, shift will voice them.
- Laterals (light blue): There are a few symbols for weird laterals sometimes used, but not all of them have unicode support so I have only included the ones on the IPA chart
- Clicks (orange)
- Approximants, Taps, and Trills (yellow)
- Implosives (pink)
- Tones (purple): to produce symbols like ˧˩˥, unicode automatically creates them when multilple tone symboles are typed consecutively. I have only included the ones with the vertical line on the right hand side, and I have not included the diacritic representations (it wouldn't fit)
- Vowels (dark green): Vowels are unrounded by default; press shift to round them. Num Lock has the front close vowels, and as you move down and to the left they become more open and further back, respectively, mimicing the ipa vowel chart. The only exceptions are that I have moved æ with ɐ, and ə with ʊ.
- Other Auxiliary Symbols (everywhere else): I have squeezed all of the auxiliary symbols included in the IPA chart into the cracks. The most common consonant diacritics are under the nasals, common vowel ones are to the right of the vowels, the symbols for prosidy are near tones, the transcription symbols and syllable break are under the arrow keys, the rest of the suprasegmentals are on Print Screen, Scroll Lock, and Pause Break, and the other random diacritics are on the so called navigation keys.

The only symbols on the official IPA chart that I haven't included are:
- ˑ "half long"
- ‿ "linking" (like with liason), but it can be emulated by using the affricate symbol.
- the diacritical symbols for tones, like ◌̋, ◌̀, ◌᷉
- The Wikipedia article for the IPA chart (https://en.wikipedia.org/wiki/International_Phonetic_Alphabet_chart) includes a few more symbols for rare laterals, but these don't have unicode support everywhere. There are also a bunch more diacritics for things like dental and schwa releases, or unrounded labialization that are in somewhat common use, but unfortunately I ran out of space.

## Installation
Because this layout overrides so many keys, it uses a AutoHotkey script. It's very easy to install, just follow this link: https://www.autohotkey.com/. To activate the script, just double click IPAkeyboard.ahk. To disable it, press Ctrl+Shift+any number key. This is because for Windows, if you have multiple keyboards installed, you can switch between them with this combination. If you want to be able to switch in to the IPA keyboard, I have also written an ahk script that just looks for Ctrl+Shift+number, where you can set the number very easily in the file. If you put default.ahk in your windows startup folder (C:\Users\<user>\AppData\Roaming\Microsoft\Windows\Start Menu\Programs) it will run automatically on startup.
