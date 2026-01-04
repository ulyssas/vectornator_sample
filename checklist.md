## Formats

- [x] format 44 (Curve Baseline)
- [x] format 14 (Vectornator Baseline)
- [x] format 40 (Monterey support, v5.7.1)
- [ ] other format

## Basics

- [x] unit tests for format 14 and 44
- [x] pixel, pica, point, inch, millimeter
- [x] multiple artboards
- [x] guide import
- [x] layer & group names
- [x] blend mode & opacity
- [x] blur effect
- [ ] shadow (maybe?)
- [x] plain path, image, group
- [x] image cropping

## Paths

- [x] node types (corner, smooth, symmetric, auto-smooth)
- [x] compound path support
- [x] proper clipping mask
- [x] stroke & fill with gradient
- [x] cornerRadius as Live Path Effect, only apply when it’s shape (star) or path
- [ ] shape support (rectangle, oval)
- [ ] line marker (circle, arrow and more)
- [x] PowerStroke

## Texts

- [x] longer Vectornator text support, uses VarInt (ULEB128)
- [x] text stroke, decoration
- [ ] text position/alignment
- [ ] textOnPath

## Architecture

- [ ] Full documentation
- [x] Python Class&Object
- [x] inkex SVG abstraction
- [x] Ignores unsupported element
- [x] type hints
- [x] Modular
- [x] Platform-independent
- [x] Inkscape extension
- [x] Online conversion via Colab
