# short-link-express
v0.0.0
<br/>

## What am I?
This respository contains short-link-express, a web application that provides short-link redirection functionality from a path to an arbitrary URL.

For example, assume this web app is hosted on example.com. In the web app code, the developer can specify that if a user visits example.com/foo, then the web app should respond with a 301 server redirection to example.org.

<br/>

<details><summary>Dev Tools</summary>

This is a web app with a server built on [Express](https://expressjs.com/) [Node.js](https://nodejs.org/en/). The source is written in [TypeScript](https://typescriptlang.org/).

| Key          | Value                                                      |
| ------------ | ---------------------------------------------------------- |
| Platform     | Windows 11                                                 |
| Architecture | amd64                                                      |
| IDE          | [Visual Studio Code](https://code.visualstudio.com/)       |
| Dependencies | See `./package.json`                                         |

</details>

<br/>

<details><summary>Deployment Infra</summary>

The source contained in this repository's `main` branch is continuously built and deployed to an [Azure Web App](https://azure.microsoft.com/en-us/services/app-service/web/) instance using [GitHub Actions](https://docs.microsoft.com/en-us/azure/app-service/deploy-github-actions?tabs=applevel).

| Key                    | Value                                             |
| ---------------------- | ------------------------------------------------- |
| Cloud Service Provider | Microsoft Azure                                   |
| Cloud App              | [Azure Web App](https://azure.microsoft.com/en-us/services/app-service/web/) |
| CI/CD Connector        | [GitHub Actions](https://docs.microsoft.com/en-us/azure/app-service/deploy-github-actions?tabs=applevel) |
| Build/Deploy Config    | See `./.github/workflows` |

</details>

<br/>
<br/>
<br/>

## Build, test, and deploy this app

### Local testing

<br/>

<details><summary>Step 1: Prepare your development environment.</summary>

1. If you don't already have Node.js, [install Node.js](https://nodejs.dev/en/learn/how-to-install-nodejs).

2. Save this Git repository on your local machine.

3. Open a terminal at the root of the repository.

4. Run the following command to install all the required Node.js packages (specified in your project root directory by `package.json`):

        npm ci

You now have:

- ... all the necessary project files downloaded to your local directory.
- ... all the necessary dependencies installed to locally build and deploy (test) this web app.

</details>

<br/>

<details><summary>Step 2: Build and run the web app.</summary>

You can now run this web app's `dev` script, which prepares a local build of the web app and deploys the build on your local host machine. It also continuously rebuilds when any changes are detected.

    npm run dev

Running the above command outputs to terminal an URL, similar to http://localhost:8080. The port number at the end varies depending on your local environment configuration.

To preview the web app, open a browser and copy-paste the output URL. (Or, in some terminals, you can directly click the URL to open a browser to that URL.)

</details>

<br/>
<br/>

### Deploying to production

<details><summary>TBD</summary>

<br/>

Placeholder for deployment instructions once on a stable minor build with continuously deploying commits.

</details>
