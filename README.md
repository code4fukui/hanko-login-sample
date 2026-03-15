# hanko-login-sample

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A sample web application that demonstrates login using the Hanko library.

## Features
- Login with Hanko, a decentralized authentication method using digital signatures
- Stores login session in browser localStorage
- Displays user's public key after successful login
- Provides a logout function to delete the stored session

## Requirements
This project requires the following to run:
- A web browser that supports ES6 modules

## Usage
1. Open the `index.html` file in a web browser.
2. Click the "Login with Hanko" button to initiate the login process.
3. After successful login, the user's public key will be displayed.
4. To logout, click the "Logout (Delete Session)" button.

## Data / API
This project uses the following external libraries:
- [Hanko](https://github.com/code4fukui/hanko/) - for decentralized authentication
- [QRCode.js](https://js.sabae.cc/QRCode.js) - for generating QR codes
- [DateTime.js](https://js.sabae.cc/DateTime.js) - for handling date and time operations
- [Base32.js](https://code4fukui.github.io/Base32/Base32.js) - for encoding session IDs

## License
This project is licensed under the MIT License.