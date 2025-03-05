# Dashlane Custom Security Dashboard Documentation

Welcome to the **Dashlane Custom Security Dashboard Documentation**. After releasing the [Dashlane Public API](https://github.com/Dashlane/public-api-documentation), we released this sample application and guide for learning and demonstration purposes. This serves as a basic introduction to using the Dashlane Public API **read-only** endpoints to access valuable insights related
to your Dashlane team account, its members and their devices.

---

## Getting Started

We’ve built a simple React application that creates a configurable security dashboard. This dashboard can be expanded to include other metrics, creating a custom dashboard so you can monitor in real time and quickly respond to credential-based risks.

1. **Clone the repository**  
   Clone [this repository](link_to_self) and download it on to your machine.

2. **Generate an API Key**  
   To communicate with our API, you’ll need an access key. Navigate to the Dashlane Admin Console > Integrations > Public API. Select “Create Key.” Give the key a description. Make sure you copy and save the bearer token in a secure place. You will not be able to access it again.

3. **Instal the dependencies**  
   Go to the cloned repository and modify the Environment variables (.env file) to add your auth token.

    ```bash
    npm install
    ```
4. **Run the dashboard**  
   To run this dashboard, just go to your preferred console, navigate to the project folder, and run:

    ```bash
    REACT_APP_DASHLANE_API_KEY="<DASHLANE BEARER TOKEN>" npm start
    ```
    A new browser window will open with your company’s custom security dashboard.

---

## Extending the dashboard

Currently, the dashboard retrieves information from the four available endpoints.

It shows user information, including password health metrics and the user’s registered devices, available from the Devices endpoint.

In addition, the dashboard shows historical and current Password Health scores, as well as the number of weak, compromised, reused, and safe passwords, available from the Password Health endpoint.

Lastly, it shows company information such as available seats and pending invitations.

Want to add more to your dashboard? The Dashlane Public API currently offers four endpoints that you can use to extend and add value to your dashboards or custom solutions.

---

## API Reference

Dashlane provides an **OpenAPI 3.0 specification** to help you explore and utilize the Public API.

-   Download the specification [here](https://get.dashlane.com/public-api/openapi.json).
-   Alternatively, use the [Documentation UI](https://dashlane.github.io/public-api-documentation/) for a user-friendly interface to explore the available endpoints.


---

## Contributing

We welcome contributions to this project! If you have ideas or enhancements, feel free to fork the repository and submit a pull request.
Please ensure that any contributions are either open source or your original work.
