# node-clipboardy

> Access the system clipboard (copy/paste)

Only for node, and original copied source code: https://github.com/sindresorhus/clipboardy

Cross-platform. Supports: macOS, Windows, Linux, OpenBSD, FreeBSD, Android with [Termux](https://termux.com/).

## Install

```sh
npm install clipboardy
```

## Usage

```js
import clipboard from 'clipboardy';

clipboard.writeSync('🦄');

clipboard.readSync();
//=> '🦄'
```

## API

### clipboard

#### .write(text)

Write (copy) to the clipboard asynchronously.

Returns a `Promise`.

##### text

Type: `string`

The text to write to the clipboard.

#### .read()

Read (paste) from the clipboard asynchronously.

Returns a `Promise`.

#### .writeSync(text)

Write (copy) to the clipboard synchronously.

##### text

Type: `string`

The text to write to the clipboard.

#### .readSync()

Read (paste) from the clipboard synchronously.