This is a fork of https://github.com/afex-connect/react-rut which adds new functionalities

# React RUT

The goal of this bundle is provide a chilean RUT utilities for [React].

## Install

with NPM:

```bash
npm install react-rut
```

with Yarn:

```bash
yarn add react-rut
```

## Usage

```tsx
import React from 'react';
import { useRut } from 'react-rut';

const Component: React.FC = () => {
  // you can set a default value with "useRut('1-9')"
  const [{ formattedValue }, setRut] = useRut();

  return (
    <input 
      onChange={(e) => setRut(e.target.value)}
      value={formattedValue}
    />
  );
};

export default Component;
```

## Testing

```bash
npm run test
```

[React](https://reactjs.org/)
