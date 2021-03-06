# [VueDiction](#) &middot; [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/chiaweilee/vue-diction/blob/master/LICENSE) [![npm version](https://img.shields.io/npm/v/vue-diction.svg?style=flat)](https://www.npmjs.com/package/vue-diction) [![npm downloads](https://img.shields.io/npm/dm/vue-diction.svg)](https://npmcharts.com/compare/vue-diction?minimal=true) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#)

🔤 Dict Component for Vue

Inspire by https://github.com/meetDeveloper/freeDictionaryAPI

* **[Pronunciation Support]:**
* **[Meanings Support]:**
* **[Origin Support]:**
* **[13 Languages Support]:**

## Example

<vue-diction word="hello"></vue-diction>

### Slot

<vue-diction word="hello">World!</vue-diction>

### Autoload

<vue-diction word="world" auto-load></vue-diction>

### Without Origin and Menanings

<vue-diction word="world" :show-origin="false" :show-meanings="false"></vue-diction>

```vue
<vue-diction word="world" :show-origin="false" :show-meanings="false"></vue-diction>
```

### Special Language

<vue-diction word="salut" language-code="fr"></vue-diction>

```vue
<vue-diction word="salut" language-code="fr"></vue-diction>
```

## Usage

### Vue Usage

```js
import VueDiction from 'vue-diction';
```

```vue
<vue-diction word="hello"></vue-diction>
```

### CDN Usage

example of docsify

```html
<script src="//cdn.jsdelivr.net/npm/vue-diction@0.3.2"></script>
<script>
  window.$docsify = {
    vueComponents: {
      'vue-diction': window.vueDiction,
    }
  };
</script>
<script src="//cdn.jsdelivr.net/npm/vue@2/dist/vue.min.js"></script>
<script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
```

### Props

|Prop|Type|Default|Description|
|:----------:|:----------:|:----------:|:----------:|
|version|Number|2||
|language-code|String|'en_GB'|'en_US', 'hi', 'es', 'fr', 'ja', 'ru', 'en_GB', 'de', 'it', 'ko', 'pt-BR', 'ar', 'tr'|
|show-origin|Boolean|true||
|show-meanings|Boolean|true||
|auto-loading|Boolean|false||

### Extend

```
<script>
  window.$docsify = {
    vueComponents: {
      'vue-diction': window.vueDictionExtend({ autoLoad: true }),
    }
  };
</script>
```