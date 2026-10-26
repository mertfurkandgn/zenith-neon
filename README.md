# Zenith Neon

A neon cyber-zen dark theme where every kind of code has its own colour, every colour passes WCAG AAA contrast and the palette holds up for colour-blind developers.

![Zenith Neon in the editor](https://raw.githubusercontent.com/mertfurkandgn/zenith-neon/main/images/screenshot.png)

## Why Zenith Neon

**15 roles, 15 colours.** Keywords, declarations, functions, types, strings, numbers, constants, variables, properties, parameters, operators, punctuation, tags, regular expressions and comments each get their own hue. You can tell what a word *is* before you read it.

**AAA contrast on everything, comments included.** Every syntax colour reaches at least 7:1 against the background, the WCAG 2.2 AAA level for body text. For comparison, none of the 17 most-installed dark themes reach 7:1 on comments, and 13 of them fall below even 4.5:1.

**Tested for colour blindness.** The palette was checked in simulations of protanopia, deuteranopia and tritanopia (Machado et al., 2009), and no two roles collapse into the same colour. Where hues come closest, style carries the meaning too: comments and parameters are italic, and function and type definitions are bold.

![The same code under a deuteranopia simulation](https://raw.githubusercontent.com/mertfurkandgn/zenith-neon/main/images/deuteranopia.png)

*Above: the same code as seen with deuteranopia, the most common form of red-green colour blindness.*

**Already familiar.** The colour roles follow what the 17 most-installed dark themes (about 81 million installs combined) mostly agree on: violet and pink keywords, blue functions, green strings, yellow types, orange numbers and neutral variables. Your habits carry over on day one.

**A quiet workspace.** The interface stays dark and low-key, and neon appears only where it carries meaning: the cursor, the active line number, errors and your code.

## Palette

| Role | Colour | Contrast | Style |
| --- | --- | --- | --- |
| Variables | `#E2E3F6` | 15.3 : 1 | |
| Regular expressions | `#D1EC32` | 14.5 : 1 | |
| Strings | `#2BFDA0` | 14.4 : 1 | |
| Types and classes | `#FDD692` | 14.0 : 1 | bold at definition |
| Operators | `#71E1FD` | 12.8 : 1 | |
| Properties | `#31DBB3` | 11.0 : 1 | |
| Parameters | `#FEAD94` | 10.7 : 1 | italic |
| Declarations (`const`, `function`, `type`) | `#D7A6FB` | 9.9 : 1 | |
| Numbers | `#FCA737` | 9.9 : 1 | |
| Functions | `#5FC2FF` | 9.8 : 1 | bold at definition |
| Constants (`true`, `null`) | `#FE8B8F` | 8.6 : 1 | |
| Control flow (`if`, `return`, `await`) | `#FC68DA` | 7.5 : 1 | |
| Punctuation | `#919DBF` | 7.2 : 1 | |
| JSX and HTML tags | `#FC6D99` | 7.2 : 1 | |
| Comments | `#A193D7` | 7.1 : 1 | italic |

Background `#0B0D18`. Contrast follows the WCAG 2.2 formula.

## Install

1. Open the Extensions view (`Ctrl+Shift+X`) and search for **Zenith Neon**.
2. Click **Install**.
3. Run **Preferences: Color Theme** (`Ctrl+K Ctrl+T`) and choose **Zenith Neon**.

Works in VS Code, Cursor, VSCodium and other editors compatible with VS Code.

## Recommended settings

```jsonc
{
  "editor.fontFamily": "'JetBrains Mono', Consolas, monospace",
  "editor.fontSize": 14,
  "editor.lineHeight": 1.4,
  "editor.letterSpacing": 0,
  "editor.semanticHighlighting.enabled": true,
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active",
  "editor.stickyScroll.enabled": true
}
```

The screenshots use exactly these settings with [JetBrains Mono](https://www.jetbrains.com/lp/mono/). Keep `editor.letterSpacing` at `0`: fractional values make selection boxes and the cursor drift away from the text on Windows at 125 % display scaling. Sticky scroll pins the enclosing function or block to the top of the editor, and the theme styles it so the current scope is always visible.

## Research basis

Zenith Neon is built on what studies actually show, including where they disagree:

- **Contrast comes first.** Legibility depends above all on the luminance contrast between text and background, which is why every role meets the AAA threshold (WCAG 2.2, SC 1.4.6).
- **Light themes have a measured edge.** Dark text on a light background gives better proofreading and detail perception, largely because the screen is brighter (Buchner & Baumgartner, 2007; Buchner et al., 2009; Piepenbrock et al., 2013, 2014), although a study with novice programmers found no performance difference between editor background styles (Park et al., 2023). Zenith Neon is a dark theme for people who prefer one, and its high contrast is there to narrow that gap.
- **Syntax colour helps, modestly.** Findings are mixed: a small benefit in one eye-tracking study (Sarkar, 2015) and no significant effect in a larger study with novices (Hannebauer et al., 2018). Distinct roles are aimed at faster scanning; no claim of large effects is made.
- **No "focus colours".** The popular idea that red sharpens attention or blue boosts creativity (Mehta & Zhu, 2009) did not replicate (Steele, 2014; Gnambs, 2020), so colours here are chosen for clarity, not mood.
- **Hue alone has limits.** Only about seven colours can be picked out reliably at a glance (Healey, 1996). With 15 roles, bold and italic back up the most important ones.

### References

- Buchner, A., & Baumgartner, N. (2007). Text–background polarity affects performance irrespective of ambient illumination and colour contrast. *Ergonomics*, 50(7). https://doi.org/10.1080/00140130701306413
- Buchner, A., Mayr, S., & Brandt, M. (2009). The advantage of positive text–background polarity is due to high display luminance. *Ergonomics*, 52(7). https://doi.org/10.1080/00140130802641635
- Gnambs, T. (2020). Limited evidence for the effect of red color on cognitive performance: A meta-analysis. *Psychonomic Bulletin & Review*, 27. https://doi.org/10.3758/s13423-020-01772-1
- Hannebauer, C., Hesenius, M., & Gruhn, V. (2018). Does syntax highlighting help programming novices? *Empirical Software Engineering*, 23. https://doi.org/10.1007/s10664-017-9579-0
- Healey, C. G. (1996). Choosing effective colours for data visualization. *Proceedings of IEEE Visualization '96*. https://doi.org/10.1109/VISUAL.1996.568118
- Machado, G. M., Oliveira, M. M., & Fernandes, L. A. F. (2009). A physiologically-based model for simulation of color vision deficiency. *IEEE TVCG*, 15(6). https://doi.org/10.1109/TVCG.2009.113
- Mehta, R., & Zhu, R. (2009). Blue or red? Exploring the effect of color on cognitive task performances. *Science*, 323(5918). https://doi.org/10.1126/science.1169144
- Park, K., Weill-Tessier, P., Brown, N. C. C., Sharif, B., Jensen, N., & Kölling, M. (2023). An eye tracking study assessing the impact of background styling in code editors on novice programmers' code understanding. *ICER '23*. https://doi.org/10.1145/3568813.3600133
- Piepenbrock, C., Mayr, S., Mund, I., & Buchner, A. (2013). Positive display polarity is advantageous for both younger and older adults. *Ergonomics*, 56(7). https://doi.org/10.1080/00140139.2013.790485
- Piepenbrock, C., Mayr, S., & Buchner, A. (2014). Positive display polarity is particularly advantageous for small character sizes. *Human Factors*, 56(5). https://doi.org/10.1177/0018720813515509
- Piepenbrock, C., Mayr, S., & Buchner, A. (2014). Smaller pupil size and better proofreading performance with positive than with negative polarity displays. *Ergonomics*, 57(11). https://doi.org/10.1080/00140139.2014.948496
- Sarkar, A. (2015). The impact of syntax colouring on program comprehension. *PPIG 2015*. https://ppig.org/files/2015-PPIG-26th-Sarkar1.pdf
- Steele, K. M. (2014). Failure to replicate the Mehta and Zhu (2009) color-priming effect on anagram solution times. *Psychonomic Bulletin & Review*, 21. https://doi.org/10.3758/s13423-013-0548-3
- W3C (2023). Web Content Accessibility Guidelines 2.2, Success Criterion 1.4.6 Contrast (Enhanced). https://www.w3.org/TR/WCAG22/#contrast-enhanced

## License

[MIT](LICENSE) © mertfurkandgn
