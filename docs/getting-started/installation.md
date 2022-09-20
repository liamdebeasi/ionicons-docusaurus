---
sidebar_position: 2
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# Installation

## Package Manager

:::note
If you are using Ionic Framework, Ionicons is packaged by default, so no installation is necessary. The steps below show how to use Ionicons without Ionic Framework.
:::

The recommended way to install `ionicons` is to use a package manager.

<Tabs>
<TabItem value="npm" label="npm">

```shell
npm install ionicons
```
</TabItem>
<TabItem value="yarn" label="Yarn">

```shell
yarn add ionicons
```
</TabItem>
</Tabs>

## CDN

Ionicons can also be loaded from a Content Delivery Network (CDN). Place the following `<script>` near the end of your page, right before the closing `</body>` tag.

```html
<script type="module" src="https://unpkg.com/ionicons/dist/ionicons/ionicons.esm.js"></script>
<script nomodule src="https://unpkg.com/ionicons/dist/ionicons/ionicons.js"></script>
```

:::note
The CDN links use the `latest` tag which always points to the latest version of Ionicons. We recommend pointing to a specific version, such as `v6.0.0`.
:::

:::note
Loading Ionicons from CDN should **not** be done in production environments. The client needs to download the entire library which can have a negative impact on performance. We recommend only loading Ionicons from CDN for prototyping or debugging purposes.
:::