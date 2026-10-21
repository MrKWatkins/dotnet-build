# dotnet-build

A reusable GitHub action for building .NET solutions. Designed for use by my other repositories.

Coverage collection and reporting are enabled by default. To run all tests without coverage, set the `coverage` input to `"false"`:

```yaml
- uses: MrKWatkins/dotnet-build@main
  with:
    coverage: "false"
```

## Pull Requests

I'm not accepting pull requests as this action is tailored for my other projects of mine.

## License

MIT
