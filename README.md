# @nutsloop/ivy-async-import-meta-resolve

___

###### async import.meta.resolve for node v20. ESModule.

___

## Index of Contents

___

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)

___

## Description

___

From Node.js v20 import.meta.resolve function is no longer a Promise.
this reinstates the fantastic async function.

___

## Installation 

___

```shell
npm install @nutsloop/ivy-async-import-meta-resolve
```

___

## Usage

___

```js

import { async_import_meta_resolve } from '@nutsloop/ivy-async-import-meta-resolve';

const path = await async_import_meta_resolve('typescript')
    .catch( error => error );
if( path instanceof Error ){
    process.stderr.write( path.message );
    process.exit( 1 );
};

process.stdout.write( path );

```

___
