# Rust Hello World ICP Project

This project demonstrates a simple "Hello, world!" canister built using Rust for the Internet Computer. The canister exposes a basic function (e.g., `greet`) that returns a greeting message when called.

---

## Table of Contents

- [Overview](#overview)
- [Deployment Instructions](#deployment-instructions)
  - [Deploying to Playground](#deploying-to-playground)
- [Testing and Verification](#testing-and-verification)
- [Submission Details](#submission-details)
- [GitHub Repository](#github-repository)

---

## Overview

This sample project was created using the command:

```bash
dfx new rust_hello --type=rust
```

It consists of a backend canister that, when its `greet` method is invoked, returns a greeting message (e.g., `"Hello, world!"`). The project can be deployed on the Internet Computer Playground, which is a test-like environment that does not consume real cycles.

---

## Deployment Instructions

### Deploying to Playground

1. **Set Up the Project Environment:**

   - Ensure you have the project cloned or set up on your machine.
   - Navigate into the project directory:
     ```bash
     cd rust_hello
     ```

2. **Deploy to the Playground Network:**

   - Use the following command to deploy the project to the Playground network:
     ```bash
     dfx deploy --network playground
     ```
   - The deployment log will display the canister IDs for both backend and frontend canisters.  
     *Note:* These canister IDs serve as evidence of successful deployment.

3. **Using the Playground Web UI (Optional):**

   - You can also deploy and test your canister through the Playground UI.
   - Visit the [ICP Playground](https://internetcomputer.org/docs/current/developer-docs/developer-tools/ide/playground/) and import your project from GitHub or copy-paste your code into the editor.
   - Use the "Deploy" button in the UI, and once deployed, the Playground will show your canister’s Candid UI and its ID.
   - Take a screenshot of the deployed canister and its Candid UI as proof of deployment.

---

## Testing and Verification

To verify that the canister is working correctly, perform the following tests:

1. **Backend Function Test:**

   - Open your terminal and run:
     ```bash
     dfx canister call rust_hello_backend greet world
     ```
   - The expected output is:
     ```
     "Hello, world!"
     ```
   - This confirms that the backend canister is functioning as intended.

2. **Frontend Verification (if applicable):**

   - If your project includes a frontend canister, use the URL provided in the deployment log (e.g., `http://127.0.0.1:4943/?canisterId=...` for local or the Playground URL).
   - Visit the URL in your browser to see the UI and capture a screenshot as additional evidence.

---

## Submission Details

When submitting your project (Wave3), please include the following:

- **Canister Evidence:**  
  - Provide the canister ID(s) displayed during deployment, **or** include a screenshot from the Playground UI showing that your canister has been successfully deployed.

- **GitHub Repository Link:**  
  - Include the URL of your GitHub repository where the code and documentation (this README) are hosted.

- **Deployment Instructions and Verification Guide:**  
  - This README contains detailed deployment instructions and a guide for verifying the canister's functionality.
  - If you used any custom deployment steps, ensure that they are clearly documented here.

---

## GitHub Repository

You can find the full project, including this README and all source code, at:

[https://github.com/yourusername/rust-hello-icp](https://github.com/yourusername/rust-hello-icp)

*Replace the above URL with the actual URL of your repository.*

---

This README provides all the required information for Wave3 submission, including the deployment procedure for the Playground environment, verification steps, and submission details.