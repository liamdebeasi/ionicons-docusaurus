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

## Variants

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
