# rn-input-mask

Text input mask for React Native on iOS and Android. (forked from https://github.com/react-native-community/react-native-text-input-mask)

<a href="https://www.npmjs.org/package/rn-input-mask">
  <img src="https://badge.fury.io/js/rn-input-mask.svg" alt="NPM package version." />
</a>
<a href="https://github.com/edstubbz/rn-input-mask/blob/master/LICENSE">
  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT license." />
</a>

## Setup

```bash
npm install --save rn-input-mask

# --- or ---

yarn add rn-input-mask
```

## Usage

```javascript
import TextInputMask from 'rn-input-mask';
...
<TextInputMask
  onChangeText={(formatted, extracted) => {
    console.log(formatted) // +1 (123) 456-78-90
    console.log(extracted) // 1234567890
  }}
  mask={"+1 ([000]) [000] [00] [00]"}
/>
...
```

## Testing

### Jest

Make sure to [mock](https://jestjs.io/docs/en/manual-mocks#mocking-node-modules) the following to `jest.setup.js`:

```javascript
jest.mock('кт-input-mask', () => ({
  default: jest.fn()
}));
```

## More info

[RedMadRobot Input Mask Android](https://github.com/RedMadRobot/input-mask-android)

[RedMadRobot Input Mask IOS](https://github.com/RedMadRobot/input-mask-ios)

## Versioning

This project uses semantic versioning: MAJOR.MINOR.PATCH.
This means that releases within the same MAJOR version are always backwards compatible. For more info see [semver.org](http://semver.org/).

## Local Development and testing

To use a local copy with your project, it's highly recommended to use https://github.com/wix/wml
