AAVE-Clone
---

## Setup and Running Locally

To get started with the project, follow these steps:

1. Copy the environment variables:
   ```sh
   cp .env.example .env.local
   ```

2. Install dependencies:
   ```sh
   yarn
   ```

3. Start the development server:
   ```sh
   yarn dev
   ```
Each commit is automatically deployed to IPFS.

A GitHub action will comment with the relevant IPFS hash linked to the Cloudflare IPFS gateway after every commit.

For convenience, you can access the latest version of the app via these links:

- [Staging environment](https://staging.aave.com) (latest IPFS hash with all networks enabled)
- [Main environment](https://app.aave.com) (latest IPFS hash with test networks disabled)

### Alternative IPFS Links:

- [https://app-aave-com.ipns.cf-ipfs.com/#/](https://app-aave-com.ipns.cf-ipfs.com/#/)
- [https://app-aave-com.ipns.dweb.link/#/](https://app-aave-com.ipns.dweb.link/#/)

### Troubleshooting

**Issue**: Unable to connect to `app.aave.com`

The Aave UI is hosted on IPFS in a decentralized manner. `app.aave.com` simply acts as a CNAME record pointing to the Cloudflare IPFS gateway. If the Cloudflare gateway is unresponsive, you can access the app via [any IPFS gateway](https://ipfs.github.io/public-gateway-checker/) that supports origin isolation.

Just visit `<your chosen public IPFS gateway>/ipns/app.aave.com`.

⚠️ Be cautious to choose a gateway that supports origin isolation to prevent security issues. The URL should look like `https://app-aave-com.<your-gateway>`.

## License

[All Rights Reserved © Aave Labs](./LICENSE.md)

## Acknowledgements

We extend our thanks to the entire Ethereum community for their ongoing contributions and support.

---

Let me know if you'd like to tweak anything further!