# FerniChat 2023
Workshop for KCDC 2023!

## Prerequisites (do before workshop)

## Installation/ setup steps
(adapted from https://docs.expo.dev/get-started/installation/)
If you regularly do JavaScript development, you likely have many of these installed already!

### Install Expo prerequisites
1. [Node.js LTS release](https://nodejs.org/en/) (version 16 or higher)
2. [Git](https://git-scm.com/). The [Github Desktop app](https://desktop.github.com/) installs this for you- that's what I use.
3. Highly recommended: [Visual Studio Code](https://code.visualstudio.com/download). Any text editor will do, but my examples will be in VS Code.
### Install CLI Tools
4. Install the Expo EAS CLI (`npm install -g eas-cli`)
5. Install Firebase CLI (`npm install -g firebase-tools`)
### Create Accounts
6. [Create an Expo Account](https://expo.dev/). Follow the link and click "Sign Up".
7. Download the "Expo Go" app on your phone from the App Store or Play Store. Sign into the app using the Expo account you just created.
8. Go to the [Firebase Console](https://console.firebase.google.com/), click "Create a Project" or "Add Project", give it a name like "[myname]-ferni-chat-2023" and accept all the default options. A Google account is required for this step.
### Fork/ Clone the demo project and restore dependencies (recommended!)
*It's a good idea to restore dependencies in case the network goes wonky during the session! Fork AND clone the repo if you'd like to push anything you do to Github. Just cloning it is fine, too, if you just want to keep everything local.*

9. Click "Fork" at the top of this page to fork the repo.
10. Clone your fork (easy way: click the green "Code" button, then "Open in Github Desktop").
11. `cd` to the folder and run `npm install`.
12. Run `npx expo login` and login with your Expo account.

## Platform-specific tips
#### Tips for Windows
- I tested this setup in Powershell and it was fine. I did have to change the execution policy first, using these instructions: https://tecadmin.net/powershell-running-scripts-is-disabled-system
- I've also worked with Expo in WSL. I followed these instructions previously to get it working with the terminal inside Visual Studio code: https://code.visualstudio.com/docs/remote/wsl
- You _may_ have to modify the Windows firewall to get the app running on your phone in the Expo Go app. If you keep getting connection timed out errors, you can try running `WF.msc` and then adding an inbound rule for port 19000.

## Verifying that everything is working
We will walk through this during the workshop, but you can also try it ahead of time to be sure that everything is installed correctly.
(adapted from https://docs.expo.dev/get-started/create-a-new-app/ - see for troubleshooting tips)
1. In the demo project folder, run `npm install`.
2. Run `npx expo start`.
3. Scan the QR code in the terminal. On iOS, scan the code with the Camera app. On Android, scan the code with the Expo Go app.
4. It should run on your phone in Expo Go (you will need to be logged in on iOS in order for this to work).
5. Alternatively (or in addition to), you can press 'w' to run the app in your browser.