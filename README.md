# react-hooks-axios

[![NPM version][npm-image]][npm-url]
[![npm download][download-image]][download-url]
[![Build Status][travis-image]][travis-url]

Custom React Hooks for [Axios.js](https://github.com/axios/axios).

## Usage

>The Hooks isn't stable, the stable release will landing on [Q1 of 2019](https://reactjs.org/blog/2018/11/27/react-16-roadmap.html). Make sure that you install the correct version of `react(>= v16.7.0-alpha)` and `react-dom(>= v16.7.0-alpha)`.

`npm i @use-hooks/axios -S`

```js
import useAxios from '@use-hooks/axios';

function YourComponent() {
  const {
    // Ref: https://goo.gl/dJ6QcV
    response,
    loading,
    error,
    // MANUAL RUN trigger
    query,
  } = useAxios({
    url: 'https://randomuser.me/api/',
    method: 'GET',
    // Ref: https://goo.gl/UPLqaK
    options: {},
    // Trigger conditions for AUTO RUN
    // trigger,
    filter: () => true,
  });

  // Others...
}
```

See [./example](https://github.com/use-hooks/react-hooks-axios/tree/master/example) for a full example.

## License

MIT

> Generated by [create-react-hooks](https://github.com/use-hooks/create-react-hooks).

 [npm-image]: https://img.shields.io/npm/v/@use-hooks/axios.svg?style=flat-square
 [npm-url]: https://npmjs.org/package/@use-hooks/axios
 [download-image]: https://img.shields.io/npm/dm/@use-hooks/axios.svg?style=flat-square
 [download-url]: https://npmjs.org/package/@use-hooks/axios
 [travis-url]: https://travis-ci.org/use-hooks/react-hooks-axios
 [travis-image]: https://img.shields.io/travis/use-hooks/react-hooks-axios.svg?style=flat-square