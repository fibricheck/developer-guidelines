# Testing

#### Libraries <a href="#testing-framework" id="testing-framework"></a>

* [testing-library/react](https://testing-library.com/docs/react-testing-library/intro/)
* [testing-library/react-native](https://testing-library.com/docs/react-native-testing-library/intro)
* [jest](https://jestjs.io/)
* [ts-jest](https://www.npmjs.com/package/ts-jest)

TODO add sample configurations

#### Unit testing

Logic that should be tested should always be extracted to util functions. This way the tested code is encapsulated and easy to test.

`TODO add example unit test`

#### Integration testing

The best coverage is achieved by writing Component integration tests that mock the network layer of the app. This way you can test the behaviour of the component in different scenarios and check that the screen shows the correct information.

The ExtraHorizon SDK exports a `getMockSdk` function that returns a mocked version of the SDK. By using this mock via Jest, you can easily mock the responses of individual calls with rejected or resolved values.

// TODO add integration test example

TODO Add visual testing lib
