import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import { logoIonic } from 'ionicons/icons';

`size="small"`: <ion-icon size="small" icon={logoIonic}></ion-icon>

`size="large"`: <ion-icon size="large" icon={logoIonic}></ion-icon>

<Tabs>
<TabItem value="angular" label="Angular">

```html title="example.component.html"
<ion-icon size="small" name="logo-ionic"></ion-icon>
<ion-icon size="large" name="logo-ionic"></ion-icon>
```
</TabItem>

<TabItem value="javascript" label="JavaScript">

```html title="index.html"
<ion-icon size="small" name="logo-ionic"></ion-icon>
<ion-icon size="large" name="logo-ionic"></ion-icon>
```
</TabItem>

<TabItem value="react" label="React">

## With Ionic Framework

```tsx title="example.tsx"
import { IonIcon } from '@ionic/react';
import { logoIonic } from 'ionicons/icons';

const Example = () => {
  return (
    <IonIcon size="small" icon={logoIonic} />
    <IonIcon size="large" icon={logoIonic} />
  );
}

export default Example;
```

## Without Ionic Framework

```tsx title="example.tsx"
import { defineCustomElement as defineIonIcon } from 'ionicons';
import { logoIonic } from 'ionicons/icons';

defineIonIcon();

const Example = () => {
  return (
    <ion-icon size="small" icon={logoIonic}></ion-icon>
    <ion-icon size="large" icon={logoIonic}></ion-icon>
  );
}

export default Example;
```
</TabItem>

<TabItem value="vue" label="Vue">

## With Ionic Framework

```html title="example.vue"
<template>
  <ion-icon size="small" :icon="logoIonic"></ion-icon>
  <ion-icon size="large" :icon="logoIonic"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { IonIcon } from '@ionic/vue';
  import { logoIonic } from 'ionicons/icons';

  export default defineComponent({
    components: { IonIcon },
    setup() {
      return { logoIonic }
    }
  });
</script>
```

## Without Ionic Framework

```html title="example.vue"
<template>
  <ion-icon size="small" :icon="logoIonic"></ion-icon>
  <ion-icon size="large" :icon="logoIonic"></ion-icon>
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