# react-native-pin-code-input

React native otp input

## Installation

```sh
npm install react-native-pin-code-input
```

## Usage

https://github.com/user-attachments/assets/c82db95f-a52d-48b2-aeb9-0eb44bd1c103


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
