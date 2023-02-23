# webhookthing sample hooks

This repository contains sample webhooks for [webhookthing](https://webhookthing.com).

## How to use

You can manually copy the `.json` files provided in this repository into your project's `.thing` directory, or you can use the webhookthing web interface to import them automatically if your `.thing` directory is empty.

## Samples

The samples in this repository are named after the service that they are for, and the event that they represent.

For example, the `github_pr_opened.json` file contains a sample payload for the webhook that is triggered when a pull request is opened on GitHub.

The contents of the `.json` files are the json body of the webhooks that are sent by the services. If you need to configure headers or query parameters, you can do so using the webhookthing web interface, or by creating a corresponding `<filename>.config.json` file with the following format:

```json
{
  "url": "https://example.com?someParam=value",
  "headers": {
    "X-Header-Name": "Header Value"
  },
  "query": {
    "someParam": "value"
  }
}
```

## Contributing

We have included a few of the more common payloads, but we are always looking to add more. If you have a payload that you would like to share, please submit a pull request!

## Issues with webhookthing? Suggestions?

If you have any issues with webhookthing, or have any suggestions for new features, we'll be using this repository's [issues](https://github.com/pingdotgg/sample_hooks/issues) to track them. Please feel free to submit any issues or suggestions you have!
