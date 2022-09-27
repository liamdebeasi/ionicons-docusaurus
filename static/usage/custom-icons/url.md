import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
<TabItem value="angular" label="Angular">

```html title="example.component.html"
<ion-icon icon="/path/to/external/file.svg"></ion-icon>
```
</TabItem>

<TabItem value="javascript" label="JavaScript">

```html
<ion-icon icon="/path/to/external/file.svg"></ion-icon>
```
</TabItem>

<TabItem value="react" label="React">

## With Ionic Framework

```tsx title="example.tsx"
import { IonIcon } from '@ionic/react';

const Example = () => {
  return <IonIcon icon="/path/to/external/file.svg" />
}

export default Example;
```

## Without Ionic Framework

```tsx title="example.tsx"
import { defineCustomElement as defineIonIcon } from 'ionicons';

defineIonIcon();

const Example = () => {
  return <ion-icon icon="/path/to/external/file.svg"></ion-icon>
}

export default Example;
```
</TabItem>

<TabItem value="vue" label="Vue">

## With Ionic Framework

```html title="example.vue"
<template>
  <ion-icon icon="/path/to/external/file.svg"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { IonIcon } from '@ionic/vue';

  export default defineComponent({
    components: { IonIcon }
  });
</script>
```

## Without Ionic Framework

```html title="example.vue"
<template>
  <ion-icon icon="/path/to/external/file.svg"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { defineCustomElement as defineIonIcon } from 'ionicons';

  export default defineComponent({
    setup() {
      defineIonIcon();
    }
  });
</script>
```
</TabItem>
</Tabs>