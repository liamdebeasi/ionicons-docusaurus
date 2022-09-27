import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import { logoIonic } from 'ionicons/icons';

<ion-icon style={{ color: 'red' }} icon={logoIonic}></ion-icon>

<Tabs>
<TabItem value="angular" label="Angular">

```html title="example.component.html"
<ion-icon name="logo-ionic"></ion-icon>
```

```css title="example.component.css"
ion-icon {
  color: red;
}
```
</TabItem>

<TabItem value="javascript" label="JavaScript">

```html
<ion-icon name="logo-ionic"></ion-icon>

<style>
  ion-icon {
    color: red;
  }
</style>
```
</TabItem>

<TabItem value="react" label="React">

## With Ionic Framework

```tsx title="example.tsx"
import { IonIcon } from '@ionic/react';
import { logoIonic } from 'ionicons/icons';

import './example.css';

const Example = () => {
  return <IonIcon icon={logoIonic} />
}

export default Example;
```

```css title="example.css"
ion-icon {
  color: red;
}
```

## Without Ionic Framework

```tsx title="example.tsx"
import { defineCustomElement as defineIonIcon } from 'ionicons';
import { logoIonic } from 'ionicons/icons';

import './example.css';

defineIonIcon();

const Example = () => {
  return <ion-icon icon={logoIonic}></ion-icon>
}

export default Example;
```

```css title="example.css"
ion-icon {
  color: red;
}
```
</TabItem>

<TabItem value="vue" label="Vue">

## With Ionic Framework

```html title="example.vue"
<template>
  <ion-icon :icon="logoIonic"></ion-icon>
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

<style scoped>
  ion-icon {
    color: red;
  }
</style>
```

## Without Ionic Framework

```html title="example.vue"
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

<style scoped>
  ion-icon {
    color: red;
  }
</style>
```
</TabItem>
</Tabs>