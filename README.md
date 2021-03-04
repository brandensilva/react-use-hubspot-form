# React Use HubSpot Form Embed

[![npm (scoped)](https://img.shields.io/npm/v/@brandensilva/react-use-hubspot-form?style=flat-square)](https://www.npmjs.com/package/@brandensilva/react-use-hubspot-form)
[![Bundle Size](https://img.shields.io/bundlephobia/min/@brandensilva/react-use-hubspot-form?style=flat-square)](https://bundlephobia.com/result?p=@brandensilva/react-use-hubspot-form)
![License](https://img.shields.io/npm/l/@brandensilva/react-use-hubspot-form?style=flat-square)

Embed HubSpot forms into your React components using hooks! Works with Create React App, Gatsby and other platforms.

## Install

```
$ npm install --save @brandensilva/react-use-hubspot-form
```

```
$ yarn add @brandensilva/react-use-hubspot-form
```

## Usage

```TypeScript
import React from 'react';

import { useHubspotForm } from '@brandensilva/react-use-hubspot-form';

const MyPage = () => {
    const { loaded, error, formCreated } = useHubspotForm({
        portalId: 'XXXXXXX',
        formId: 'XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX',
        target: '#my-hubspot-form'
    });

    return (
        <div>
            <h1>Embed Form Below</h1>
            <div id="my-hubspot-form"></div>
        </div>
    )
}

```
