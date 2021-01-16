# :warning::warning: DEPRECATED :warning::warning:

This project, and it's related TestArmada projects, will no longer be supported. No further work from the owners will be done, and no PRs will be reviewed.

# Magellan JSON Reporter Plugin

This project is a plugin for Magellan which allows you to report test information in a JSON file.

# Installation

Install the npm module in your node project:

```shell
npm install --save testarmada-magellan-json-reporter
```

Add the plugin to `magellan.json` in the `reporters` list (note: if this file doesn't exist, create it)

```json
{
  "reporters": [
    "testarmada-magellan-json-reporter"
  ]
}
```

# Configuration

This plugin is configured with environment variables.

- `JSON_REPORT_PATH` - path name where to put the JSON report file, e.g. `./mocha_report.json`

# Limitation
Currently to see the error stack trace in JSON report:
* add `--reporter json` into your `mocha.opts` file
* use Magellan version >=8.6.0
* Magellan option `--max_test_attempts` cannot be set to 1

## License
Documentation in this project is licensed under Creative Commons Attribution 4.0 International License. Full details available at https://creativecommons.org/licenses/by/4.0
