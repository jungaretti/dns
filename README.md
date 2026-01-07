# DNS Records

All of my DNS records, deployed with [Bacon](https://github.com/jungaretti/bacon).

## Getting Started

I use the [Deploy with Bacon](https://github.com/jungaretti/bacon-deploy-action) action to deploy DNS records from this repo to [Porkbun](https://porkbun.com/). To learn more about Bacon and its deploy action, see these repos:

- [jungaretti/bacon](https://github.com/jungaretti/bacon)
- [jungaretti/bacon-deploy-action](https://github.com/jungaretti/bacon-deploy-action)

### How to Deploy a New Domain

1. [Enable API access for the domain on Porkbun](https://kb.porkbun.com/article/190-getting-started-with-the-porkbun-api)
2. Create a new YAML file in the [`dns`](./dns/) directory
3. Add a step to each workflow file
   - [`bacon-deploy.yml`](.github/workflows/bacon-deploy.yml)
   - [`bacon-deploy-preview.yml`](.github/workflows/bacon-deploy-preview.yml)
4. Make a pull request to preview deployment
5. Merge the pull request to trigger deployment

### Update an Existing Domain

1. Update a YAML file in the [`dns`](./dns/) directory
2. Make a pull request to preview deployment
3. Merge the pull request to trigger deployment
