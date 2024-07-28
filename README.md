# Card image generator

Used it for a custom Brave Rats retheme. Code is entirely throwaway at the moment, so temper your expectations. Most
everything is hardcoded, so to use this you'd edit `index.html` and open it in a browser. (NOTE: the various art assets
referenced are intentionally omitted to avoid any legal issues) 

The basic idea is to assemble the desired output in an HTML element, then render that to a canvas, then save that to an
image. This makes it pretty easy to apply fairly advanced effects (to text or otherwise) and quickly check the layout of
various cards.

To change which card is shown, press the left/right cursor keys, or use up/down to switch between blue and red.
Pressing `S` lets you save the current card to a file, and `A` will save ALL cards.
(The summary cards are a different beast entirely, they're on their separate branch `summary_card` for now)

# Print-and-play process

Some additional notes below for various tools used in my process.

For creating the background images, [GIMP][gimp] (and dozens of hours).
For content-aware fill, [Pincel][fill] worked well enough as a free option.
For interpolating colors, [this website][blend] was handy. Seemed to look better than just reducing opacity.

For aligning the card elements properly, this [template][template] (and [explanatory video][explain]).
size template: export from inkscape (find the original?)
For generating a printable PDF from the individual card images, [PnPBuddy][pnp].
For setting up a print-on-demand order, [MPC Autofill][autofill].

[template]: https://goo.gl/by1eqJ
[explain]:  https://www.youtube.com/watch?v=XbP1QLcOlYE
[autofill]: https://mpcfill.com/editor
[pnp]:      http://www.pnpbuddy.com/layout/
[gimp]:     https://www.gimp.org/
[fill]:     https://pincel.app/tools/inpaint
[blend]:    https://meyerweb.com/eric/tools/color-blend/
