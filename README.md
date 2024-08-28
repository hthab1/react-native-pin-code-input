# react-native-pin-code-input

React native otp input

## Installation

```sh
npm install react-native-pin-code-input
```

## Usage


```js
import OTPInput from 'react-native-pin-code-input';

// ...

export default function App() {
  const [otp, setOtp] = useState<string>('');
  return (
    <View style={styles.container}>
      <OTPInput
        containerStyle={{ width: '90%' }}
        autoFocus
        pinCount={6}
        onOtpFilled={(code) => setOtp(code)}
      />
      {otp && <Text>Your OTP is {otp}</Text>}
    </View>
  );
}
```


## Contributing

See the [contributing guide](CONTRIBUTING.md) to learn how to contribute to the repository and the development workflow.

## License

MIT

---

Made with [create-react-native-library](https://github.com/callstack/react-native-builder-bob)
