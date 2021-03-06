# Angular IMask Plugin
angular-imask

[![npm version](https://badge.fury.io/js/angular-imask.svg)](https://badge.fury.io/js/angular-imask)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Install
`npm install angular-imask`

## Setup
```javascript
import {IMaskModule} from 'angular-imask';

@NgModule({
  imports: [
    IMaskModule,
    ...
  ],
  ...
}) {...}
```

## Usage
```html
<input
  [imask]="{mask: '+{7}(000)000-00-00'}"  <!--see more mask props in a guide-->
  [unmask]="true"  <!--optionally use `unmaskedValue` or `value` otherwise-->
  (accept)="onAccept"  <!--first argument is `value` or `unmaskedValue` depending on prop above-->
  (complete)="onComplete"
/>
```
More options see in a [guide](https://unmanner.github.io/imaskjs/guide.html).
