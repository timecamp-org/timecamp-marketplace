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
    "release_date": string, // format: YYYY-MM-DD
    "icon_url": string,
    "categories": string[], // any of "report", "plugin", "tool", "integration", "featured"
    "repo": string, // optional
    "price": string, // optional
    "update_date": string, // optional, format: YYYY-MM-DD
    "api_url": string, // optional
    "url": string, // optional
}
```

## API URL (optional)

It should have the following endpoints:

- Enable item
- Disable item
- Is enabled
