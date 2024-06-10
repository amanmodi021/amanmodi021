

![Bopis](gitbanner2.png)

<a href="https://www.hotwax.co/"><img alt="HOTWAX" src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social"></a>
[![Website](https://raw.githubusercontent.com/praveenscience/praveenscience/master/soc/ws.svg)](https://praveen.science/) 

[![Blog](https://raw.githubusercontent.com/praveenscience/praveenscience/master/soc/bl.svg)](https://blog.praveen.science/) 

[![LinkedIn](https://raw.githubusercontent.com/praveenscience/praveenscience/master/soc/li.svg)](https://uk.linkedin.com/in/praveentech/) 

[![Twitter](https://raw.githubusercontent.com/praveenscience/praveenscience/master/soc/tw.svg)](https://twitter.com/praveenscience) 

[![YouTube](https://raw.githubusercontent.com/praveenscience/praveenscience/master/soc/yt.svg)](https://youtube.com/praveenscience)


# Bopis App - Buy Online and Pickup at Store
##   Effortlessly combine online shopping with convenient in-store pickup for a superior retail experience


# Introduction

BOPIS App: A Seamless Buy Online, Pick Up In-Store Solution
Our BOPIS (Buy Online, Pick Up In-Store) app enhances the retail shopping experience by combining the convenience of online shopping with the immediacy of in-store pickup. Perfect for modern shoppers and retailers alike, this app offers a flexible and efficient solution for purchasing and collecting goods.
## Key Features of the BOPIS App:
- **Product Browsing**: Easily explore a wide range of products available at nearby store locations.
- **Real-Time Inventory**: Stay updated with live stock levels to ensure items are available for immediate pickup.
- **Seamless Order Placement**: Enjoy a smooth online ordering process with secure payment options.
- **Convenient Store Selection**: Choose the most convenient pickup location based on proximity and product availability.
- **Flexible Pickup Scheduling**: Select your preferred pickup time to match your schedule.
- **Timely Notifications**: Receive alerts and updates on your order status and readiness for pickup.
- **Robust Customer Support**: Access assistance and answers to common questions through chat or call features.
  
By bridging the gap between digital and physical retail, our BOPIS app provides a comprehensive and user-friendly shopping alternative that boosts customer satisfaction and streamlines operations for retailers.





![Bopis](BOPISgit.png)

# Prerequisite
Ionic CLI - If you don't have the ionic CLI installed refer [official documentation](https://ionicframework.com/docs/intro/cli) for the installation instructions.


# Build Notes- Users

1. Download the app from [release](https://github.com/hotwax/bopis/releases) page and extract it.
2. Go to the app directory.
3. Run following command to download dependencies  
    `npm i`
4. Create a `.env` file by taking reference from the `.env.example` and set the `VUE_APP_BASE_URL` to the instance you want to connect the app.
5. To run the app in browser use the command: `ionic serve`


# Build Notes- Contributors

1. Open a Terminal window
2. Clone app using the command: `git clone https://github.com/hotwax/bopis.git <repository-name>`
3. Go to the <repository-name> directory using command: `cd <repository-name>`
4. Run following command to download dependencies
    `npm i`
5. Create a `.env` file by taking reference from the `.env.example` and change the `VUE_APP_BASE_URL` to the instance you want to connect the app.
6. To run the app in browser use the command: `ionic serve`

## Firebase Hosting

We are using firebase hosting for the Bopis app deployment
Here are the steps to deploy app on firebase hosting

### Prerequisite

- [Firebase Cli](https://firebase.google.com/docs/cli) should be installed
- Firebase project should be created
- You should have access to firebase project

### Dev Deployment

- Update the DEV instance url at .env.production file

- Build the application using following command
  `ionic build`

- Login into firebase
  `firebase login`

- Run following command to deploy to firebase hosting
  `firebase deploy --only hosting:sm-dev`

## How to Build Application in Different Environment or Modes(Development, UAT, Production etc)?

As there is a bug in Ionic cli due to which we cannot pass flag variables for commands (See [#4669](https://github.com/ionic-team/ionic-cli/issues/4642)). To build application in different modes we need to use vue-cli-service to build and then use the built app using capacitor copy command further.

Follow following instructions:

1. Manually build the application using vue-cli-service:
   npx vue-cli-service build --mode=sandbox

2. Copy web assets to the native project without building the app:
   ionic capacitor copy ios --no-build

3. Open the Android Studio / XCode project:
   ionic capacitor open android  
   ionic capacitor open ios

# Contribution Guideline

1. Fork the repository and clone it locally from the `main` branch. Before starting your work make sure it's up to date with current `main` branch.
2. Pick an issue from [here](https://github.com/hotwax/bopis/issues). Write in the issue comment that you want to pick it, if you can't assign yourself. **Please stay assigned to one issue at a time to not block others**.
3. Create a branch for your edits. Use the following branch naming conventions: **bopis/issue-number**.
4. Please add issue number to your commit message.
5. Propose a Pull Request to `main` branch containing issue number and issue title.
6. Use [Pull Request template](https://github.com/hotwax/bopis/blob/main/.github/PULL_REQUEST_TEMPLATE.md) (it's automatically added to each PR) and fill as much fields as possible to describe your solution.
7. Reference any relevant issues or other information in your PR.
8. Wait for review and adjust your PR according to it.
9. Congrats! Your PR should now be merged in!

If you can't handle some parts of the issue then please ask for help in the comment. If you have any problems during the implementation of some complex issue, feel free to implement just a part of it.

# Report a Bug or Request a Feature

Always define the type of issue:
* Bug report
* Feature request

While writing issues, please be as specific as possible. All requests regarding support with implementation or application setup should be sent to.
# UI/UX Resources
You may find some useful resources for improving the UI / UX of the app <a href="https://www.figma.com/community/file/885791511781717756" target="_blank">here</a>.

# Join the Community on Discord
If you have any questions or ideas feel free to join our <a href="https://discord.gg/SwpJnpdyg3" target="_blank">Discord channel</a>.
    
# The License

Bopis app is completely free and released under the Apache v2.0 License. Check <a href="https://github.com/hotwax/bopis/blob/main/LICENSE" target="_blank">LICENSE</a> for more details.
