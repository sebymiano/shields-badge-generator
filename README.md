# Shileds.io Badge Generator
![.github/workflows/test.yml](https://github.com/sebymiano/shields-badge-generator/blob/badges/main/test.svg)

This action generates a SVG badge from [Shields.io](https://shields.io/) and saves it to a file.

## Inputs

### `label`

**Required** The left label of the badge, usually static.

### `status`

**Required** The right status as the badge, usually based on results.

### `color`

**Required** An array (comma separated) with hex or named colors of the badge value background. More than one creates gradient background. Default: `blue`.

### `label-color`

**Required** Hex or named color of the badge label. Default: `555`.

### `style`

**Required** Badge style: `flat`, `flat-square`, `plastic`, `for-the-badge`, `social`. Default: `flat`.

### `logo`

One of the named logos or simple-icons. See [simpleicons](https://simpleicons.org/). Default: `none`.

### `logo-color`

The color of the logo (hex, rgb, rgba, hsl, hsla and css named colors supported).

### `path`

**Required** The file path to store the SVG badge file.

## Example usage

```
uses: sebymiano/shields-badge-generator@v1.0.3
with:
  label: 'Docker build'
  status: 'Success'
  color: 'green'
  logo: 'docker'
  path: '.github/badges/docker-build.svg'
```