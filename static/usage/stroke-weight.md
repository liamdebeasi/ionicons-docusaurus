import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import { heartOutline } from 'ionicons/icons';

<ion-icon style={{ '--ionicon-stroke-width': '48px' }}icon={heartOutline}></ion-icon>

<Tabs>
<TabItem value="angular" label="Angular">

```html title="example.component.html"
<ion-icon name="heart-outline"></ion-icon>
```

```css title="example.component.css"
ion-icon {
  --ionicon-stroke-width: 48px;
}
```
</TabItem>

<TabItem value="javascript" label="JavaScript">

```html
<ion-icon name="heart-outline"></ion-icon>

<style>
  ion-icon {
    --ionicon-stroke-width: 48px;
  }
</style>
```
</TabItem>

<TabItem value="react" label="React">

## With Ionic Framework

```tsx title="example.tsx"
import { IonIcon } from '@ionic/react';
import { heartOutline } from 'ionicons/icons';

import './example.css';

const Example = () => {
  return <IonIcon icon={heartOutline} />
}

export default Example;
```

```css title="example.css"
ion-icon {
  --ionicon-stroke-width: 48px;
}
```

## Without Ionic Framework

```tsx title="example.tsx"
import { defineCustomElement as defineIonIcon } from 'ionicons';
import { heartOutline } from 'ionicons/icons';

import './example.css';

defineIonIcon();

const Example = () => {
  return <ion-icon icon={heartOutline}></ion-icon>
}

export default Example;
```

```css title="example.css"
ion-icon {
  --ionicon-stroke-width: 48px;
}
```
</TabItem>

<TabItem value="vue" label="Vue">

## With Ionic Framework

```html title="example.vue"
<template>
  <ion-icon :icon="heartOutline"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { IonIcon } from '@ionic/vue';
  import { heartOutline } from 'ionicons/icons';

  export default defineComponent({
    components: { IonIcon },
    setup() {
      return { heartOutline }
    }
  });
</script>

<style scoped>
  ion-icon {
    --ionicon-stroke-width: 48px;
  }
</style>
```

## Without Ionic Framework

```html title="example.vue"
<template>
  <ion-icon :icon="heartOutline"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { defineCustomElement as defineIonIcon } from 'ionicons';
  import { heartOutline } from 'ionicons/icons';

  export default defineComponent({
    setup() {
      defineIonIcon();
      return { heartOutline }
    }
  });
</script>

<style scoped>
  ion-icon {
    --ionicon-stroke-width: 48px;
  }
</style>
```
</TabItem>
</Tabs>