---
sidebar_position: 2
---

import { defineCustomElement } from 'ionicons/components/ion-icon.js';
defineCustomElement();

# Developing

TODO Developing

## Basic Usage

import BasicUsage from '@site/static/usage/basic-usage.md';

<BasicUsage />

## Custom Icons

### With a URL

To load a custom SVG from a URL, pass the URL to the `icon` property. Make sure that the file is accessible from the webpage that is making the request. For security reasons, Ionicons does not allow scripts or events within the custom SVG element.

import CustomURL from '@site/static/usage/custom-icons/url.md';

<CustomURL />

### With SVG Data

Developers can also pass the raw SVG data to the `icon` property. For security reasons, Ionicons does not allow scripts or events within the custom SVG element.

import CustomData from '@site/static/usage/custom-icons/data.md';

<CustomData />

## Variants

Each app icon in Ionicons has a `filled`, `outline`, and `sharp` variant. These different variants are provided to make your app feel native to a variety of platforms. The filled variant uses the default name without a suffix. Note: Logo icons do not have outline or sharp variants.

import Variants from '@site/static/usage/variants.md';

<Variants />

## Size

To specify the icon size, use the `size` property for pre-defined icon sizes.

import Size from '@site/static/usage/size.md';

<Size />

## Color

Specify the icon color by applying the `color` CSS property on the `ion-icon` component.

import Color from '@site/static/usage/color.md';

<Color />

## Stroke Weight

When using an `outlin`e icon variant it is possible to adjust the stroke weight, for improved visual balance relative to the icon's size or relative to the weight of adjacent text. You can set a specific size by applying the `--ionicon-stroke-weight` CSS custom property to the ion-icon component. The default value is `32px`.

import StrokeWeight from '@site/static/usage/stroke-weight.md';

<StrokeWeight />
