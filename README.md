# fabble-data

Generated dataset for [Fabble](https://fabkit.io/#/fabble), served via GitHub
Pages at:

```
https://fabkit.github.io/fabble-data/v1/dataset.json
```

**This repo holds generated files only — do not edit them by hand.**

Source pipeline: [FABKIT/fabble-admin](https://github.com/FABKIT/fabble-admin)
(private). A GitHub Action there rebuilds and pushes `v1/dataset.json` here
on a schedule (Monday + Thursday UTC) and on manual dispatch.

The `v1/` path segment is a schema-version escape hatch — if the app's
`FabbleDataset.schemaVersion` ever needs to become `2`, that publishes to a
new `v2/` path so old clients keep working against `v1/` until they update.
