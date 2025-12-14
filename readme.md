# TimeCamp Marketplace

This is the TimeCamp Marketplace. It is a collection of items that can be installed in TimeCamp.

## Adding an item to the marketplace

Add new pull request to the `timecamp-marketplace-items.json` file.

JSON schema:

```json
{
    "id": string,
    "name": string,
    "author": string,
    "description": string,
    "icon_url": string,
    "categories": string[], // any of "report", "plugin", "tool", "integration"
    "repo": string, // optional
    "price": string, // optional
    "api_url": string, // optional
    "url": string, // optional
}
```

## API URL (optional)

It should have the following endpoints:

- Enable item
- Disable item
- Is enabled
