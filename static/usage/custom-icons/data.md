import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
<TabItem value="angular" label="Angular">

```html title="example.component.html"
<ion-icon [icon]="customIcon"></ion-icon>
```

```typescript title="example.component.ts"
import { Component } from '@angular/core';
import svgData from '/path/to/external/file.svg';

@Component({
  selector: 'app-example',
  templateUrl: 'example.component.html',
})
export class ExampleComponent {
  public customIcon = svgData;
  constructor() {}
}

```
</TabItem>

<TabItem value="javascript" label="JavaScript">

```html
<ion-icon icon="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg'>...</svg>"></ion-icon>
```
</TabItem>

<TabItem value="react" label="React">

## With Ionic Framework

```tsx title="example.tsx"
import { IonIcon } from '@ionic/react';
import svgData from '/path/to/external/file.svg';

const Example = () => {
  return <IonIcon icon={svgData} />
}

export default Example;
```

## Without Ionic Framework

```tsx title="example.tsx"
import { defineCustomElement as defineIonIcon } from 'ionicons';
import svgData from '/path/to/external/file.svg';

defineIonIcon();

const Example = () => {
  return <ion-icon icon={svgData}></ion-icon>
}

export default Example;
```
</TabItem>

<TabItem value="vue" label="Vue">

## With Ionic Framework

```html title="example.vue"
<template>
  <ion-icon :icon="svgData"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { IonIcon } from '@ionic/vue';
  import svgData from '/path/to/external/file.svg';

  export default defineComponent({
    components: { IonIcon },
    setup() {
      return { svgData };
    }
  });
</script>
```

## Without Ionic Framework

```html title="example.vue"
<template>
  <ion-icon :icon="svgData"></ion-icon>
</template>

<script>
  import { defineComponent } from 'vue';
  import { defineCustomElement as defineIonIcon } from 'ionicons';
  import svgData from '/path/to/external/file.svg';

  export default defineComponent({
    setup() {
      defineIonIcon();
      return { svgData };
    }
  });
</script>
```
</TabItem>
</Tabs>