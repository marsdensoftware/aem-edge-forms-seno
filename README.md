# Your Project's Title...

## Environments

- Preview: https://main--edge-forms-seno--marsdensoftware.aem.page/
- Live: https://main--edge-forms-seno--marsdensoftware.aem.live/

## Documentation

Before using the aem-boilerplate, we recommand you to go through the documentation on [www.aem.live](https://www.aem.live/docs/) and [experienceleague.adobe.com](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/edge-delivery/wysiwyg-authoring/authoring), more specifically:

-[Getting Started – Universal Editor Developer Tutorial](https://www.aem.live/developer/ue-tutorial)

- [Getting Started Guide](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/edge-delivery/wysiwyg-authoring/edge-dev-getting-started)
- [Creating Blocks](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/edge-delivery/wysiwyg-authoring/create-block)
- [Content Modelling](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/edge-delivery/wysiwyg-authoring/content-modeling)
- [Working with Tabular Data / Spreadsheets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/edge-delivery/wysiwyg-authoring/tabular-data)

Furthremore, we encourage you to watch the recordings of any of our previous presentations or sessions:

- [Getting started with AEM Forms Authoring and Edge Delivery Services](https://experienceleague.adobe.com/en/docs/events/experience-manager-gems-recordings/gems2024/edge-delivery-for-aem-forms)

## Prerequisites

- nodejs 18.3.x or newer
- AEM Cloud Service release 2024.8 or newer (>= `17465`)

## Installation

```sh
npm i
```

## Linting

```sh
npm run lint
```

## Local development

1. Create a new repository based on the `aem-boilerplate` template and add a mountpoint in the `fstab.yaml`
   i.e `https://<aem-author>/bin/franklin.delivery/<owner>/<repository>/main`
2. Change mapping url in `paths.json`
   i.e

```json
{
  "mappings": [
    "/content/[your-site-name]/:/",
    "/content/[your-site-name]/configuration:/.helix/config.json",
    "/content/[your-site-name]/metadata:/metadata.json"
  ],
  "includes": ["/content/[your-site-name]/"]
}
```

3. Add the [AEM Code Sync GitHub App](https://github.com/apps/aem-code-sync) to the repository
4. Install the [AEM CLI](https://github.com/adobe/helix-cli): `npm install -g @adobe/aem-cli`
5. Start AEM Proxy: `aem up` (opens your browser at `http://localhost:3000`)
6. Open the `{repo}` directory in your favorite IDE and start coding
