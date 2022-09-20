---
sidebar_position: 1
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import { logoIonic } from 'ionicons/icons';
import { defineCustomElement } from 'ionicons/components/ion-icon.js';
defineCustomElement();

# Basic Usage

<ion-icon icon={logoIonic}></ion-icon>

<Tabs>
<TabItem value="angular" label="Angular">

```html
<ion-icon name="logo-ionic"></ion-icon>
```
</TabItem>

<TabItem value="javascript" label="JavaScript">

```html
<ion-icon name="logo-ionic"></ion-icon>
```
</TabItem>

<TabItem value="react" label="React">

```tsx title="With Ionic Framework"
import { IonIcon } from '@ionic/react';
import { logoIonic } from 'ionicons/icons';

const Example = () => {
  return <IonIcon icon={logoIonic} />
}

export default Example;
```

```tsx title="Without Ionic Framework"
import { defineCustomElement as defineIonIcon } from 'ionicons';
import { logoIonic } from 'ionicons/icons';

defineIonIcon();

const Example = () => {
  return <ion-icon icon={logoIonic}></ion-icon>
}

export default Example;
```
</TabItem>

<TabItem value="vue" label="Vue">

```html title="With Ionic Framework"
<template>
  <ion-icon :icon="logoIonic"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { IonIcon } from 'ionicons';
  import { logoIonic } from 'ionicons/icons';

  export default defineComponent({
    components: { IonIcon },
    setup() {
      return { logoIonic }
    }
  });
</script>
```

```html title="Without Ionic Framework"
<template>
  <ion-icon :icon="logoIonic"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { defineCustomElement as defineIonIcon } from 'ionicons';
  import { logoIonic } from 'ionicons/icons';

  export default defineComponent({
    setup() {
      defineIonIcon();
      return { logoIonic }
    }
  });
</script>
```
</TabItem>
</Tabs>