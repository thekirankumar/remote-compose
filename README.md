# KITE - Remote Compose Demo

This project is a demonstration of using **Remote Compose**, a server-driven UI paradigm for Jetpack Compose. Remote Compose allows you to define and update your application's UI from a remote source, without needing to release a new version of your app.

## About Remote Compose

As described in the article [RemoteCompose - Another Paradigm for Server-Driven UI in Jetpack Compose](https://proandroiddev.com/remotecompose-another-paradigm-for-server-driven-ui-in-jetpack-compose-92186619ba8f), this technology works by transmitting a description of a Composable UI (as a `CoreDocument`) from a server to the client. The client then uses the `RemoteDocumentPlayer` to render the UI natively.

This approach is powerful for situations where the UI needs to be changed frequently, such as:
- A/B testing different layouts
- Rolling out new UI features dynamically
- Displaying dynamic content from a CMS

## Demo

![Demo GIF](github/demo.gif)

## Running This Project

This is a standard Android Studio project. You can clone it, open it in Android Studio, and run it on an emulator or a physical device to see a simple implementation of a remotely-rendered UI.

## Key Dependencies

This project utilizes snapshot versions of the following key Remote Compose libraries:
- `remote-player-compose`
- `remote-core`
- `remote-tooling-preview`

## Attribution

The sample applications in this project are based (copied!) from the integration tests for Remote Compose from the Android Open Source Project. You can find the original source code [here](https://android.googlesource.com/platform/frameworks/support/+/androidx-main/compose/remote/integration-tests/).
