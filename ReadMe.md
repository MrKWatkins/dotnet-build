# dotnet-build

A reusable GitHub action for building .NET solutions. Designed for use by my other repositories.

Coverage collection and reporting are enabled by default. To run all tests without coverage, set the `coverage` input to `"false"`:

```yaml
- uses: MrKWatkins/dotnet-build@main
  with:
    coverage: "false"
```

Tests run without filtering by default. Set `test-filter` to pass a filter expression to `dotnet test`. For example, to exclude selected NUnit categories:

```yaml
- uses: MrKWatkins/dotnet-build@main
  with:
    test-filter: "TestCategory!=LinearScan&TestCategory!=Unoptimized&TestCategory!=Slow"
```

The filter is passed as a single argument, including any spaces or operators. Omitting it leaves existing consumers unchanged.

## Pull Requests

I'm not accepting pull requests as this action is tailored for my other projects of mine.

## License

MIT
