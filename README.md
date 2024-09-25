# Ruby DuckDB Buildpack

This buildpack installs DuckDB for your Ruby project using buildpacks.

## How to Use

To use this buildpack in your project, follow these steps:

1. Add the buildpack to your `project.toml` file in your project repository:

   ```toml
   [[build.buildpacks]]
   uri = "fagianijunior/ruby-duckdb"
   ```

2. Add the following variable to your environment:

   ```
   BUNDLE_BUILD__DUCKDB="--with-duckdb-include=/app/vendor/duckdb/include --with-duckdb-lib=/app/vendor/duckdb/lib"
   ```   ```

3. Deploy your application as usual.

## DuckDB Version

This buildpack installs DuckDB version 1.1.0. If you need a different version, please open an issue or submit a pull request.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
