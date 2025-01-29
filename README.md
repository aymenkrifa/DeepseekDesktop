# DeepSeek Linux Desktop Client

A simple Electron based desktop client for DeepSeek Linux. No need to open a browser to access DeepSeek Linux. Just download and install the client and you are good to go.

## Dependencies

- Node.js
- Electron

## Installation

1. Clone the repository
2. Run `npm install`
3. Run `npm run start`

If you want to package the Electron app, run the following command:

```bash
npx electron-packager . --platform=linux --arch=x64 --out=dist --icon=assets/icon.png --overwrite
```

If you want to create an AppImage for the Electron app, copy the `deepseek.desktop` file to your `~/.local/share/applications` directory (make sure to change the `Exec` path to the absolute path of the AppImage file)

If the path to my AppImage file is `/home/user/deepseekdesktop/dist/deepseek-chat-app-linux-x64/deepseek-chat-app`, then the `Exec` path in the `deepseek.desktop` file should be `/home/user/deepseekdesktop/dist/deepseek-chat-app-linux-x64/deepseek-chat-app`

Make sure to add execute permissions to the AppImage file by running `chmod +x /home/user/deepseekdesktop/dist/deepseek-chat-app-linux-x64/deepseek-chat-app`
