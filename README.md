# Box Template Generator

A free, printable box template generator. Enter the finished size of the box you want, preview the cut-and-fold net as SVG, then print it at true size or download the SVG.

**Live demo:** https://toolnestcalc.com/box-template-generator/

## What it does

- One-piece glued gift box net (base, four walls, optional lid) with trapezoidal glue tabs
- Units: inches, centimetres, millimetres
- Presets: small gift, favour box, large gift
- Net size calculation and a fits-on-page check for US Letter and A4, including a fit-to-page scale with the finished size at that scale
- Print at 100 percent with a 1 inch / 25 mm scale-check line, or download the net as SVG
- Cut on solid lines, score and fold on dashed lines

## How the net works

The net is a cross net: the base sits in the middle, one wall folds up from each of its four edges, and the lid hangs off the bottom wall. For a box of length L, width W and height H, the full net measures L + 2H across and 2W + 2H tall before the glue tabs (plus one more W of height when the lid is on). That is why even a modest box can outgrow one sheet of paper.

The core geometry lives in `computeNet()` and `fitInfo()` in `index.html`, with no dependencies. The same functions are exported for Node (`module.exports`) so the geometry can be unit-tested without a browser.

## Use

Open `index.html` in any browser. No build step, no backend, no dependencies. Defaults: 3 x 2.5 x 1.5 in, lid on, US Letter at 100 percent, giving a net size of 7.10 in x 8.00 in.

## Scope

This covers the one-piece paper and card gift box net only. Tuck-end cartons, two-piece lift-off lids and laser-cut finger-joint boxes use different geometry and are not covered here.

## License

MIT. See `LICENSE`.
