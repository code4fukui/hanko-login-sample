# hanko-login-sample

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A sample web application demonstrating a client-side login flow using [Hanko](https://github.com/code4fukui/hanko/), a decentralized authentication method based on digital signatures.

## Demo

A live demo is available at: **[https://code4fukui.github.io/hanko-login-sample/](https://code4fukui.github.io/hanko-login-sample/)**

## How It Works

This sample demonstrates a complete client-side authentication loop:

1.  The user clicks the login button on this sample app ("何かのサービス" / "Some Service").
2.  The app opens the Hanko web app in a new tab with a message to be signed.
3.  The user authenticates and signs the message within the Hanko app.
4.  Hanko redirects the user back to this sample app, passing the signature in the URL.
5.  The sample app's JavaScript verifies the signature, its content, and its timestamp.
6.  On successful verification, a session is created in `localStorage`, and the user's public key is displayed.

## Features

-   **Decentralized Login:** Authenticate users via the Hanko digital signature flow.
-   **Session Persistence:** Stores the user session in the browser's `localStorage`.
-   **User Identification:** Displays the user's public key (DID) after a successful login.
-   **Logout:** Clears the session from `localStorage`.

## Requirements

-   A modern web browser that supports ES6 modules.

## Usage

1.  Open the `index.html` file in a web browser or visit the demo URL.
2.  Click the **"Hankoでログイン"** (Login with Hanko) button.
3.  In the new tab, use the Hanko app to sign the login request.
4.  After signing, you will be redirected back to the sample application.
5.  Upon successful login, a welcome message with your public key will be displayed.
6.  To log out, click the **"ログアウト（セッション削除）"** (Logout (Delete Session)) button.

## Dependencies

This project relies on the following external libraries:
-   [Hanko](https://github.com/code4fukui/hanko/) - For decentralized authentication.
-   [QRCode.js](https://js.sabae.cc/QRCode.js) - For generating QR codes.
-   [DateTime.js](https://js.sabae.cc/DateTime.js) - For handling date and time operations.
-   [Base32.js](https://code4fukui.github.io/Base32/Base32.js) - For encoding session IDs.

## License

MIT License — see [LICENSE](LICENSE).