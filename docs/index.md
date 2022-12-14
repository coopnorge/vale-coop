# Coop Vale Package

Vale Style Package for Coop.

## Usage

Add a `.vale.ini` to your repository.

```ini title=".vale.ini"
StylesPath = .vale/styles

Packages = https://github.com/coopnorge/vale-coop/releases/latest/download/Coop.zip
```

Repository specific Configuration can also be added.

```ini title=".vale.ini"
StylesPath = .vale/styles

Packages = https://github.com/coopnorge/vale-coop/releases/latest/download/Coop.zip

Vocab = Norwegian

[*.md]
TokenIgnores = coop\.no, https://teams.microsoft.com/l/channel/
```

The example above adds a local [vocabulary](https://vale.sh/docs/topics/vocab/)
that vale will look for in `.vale/style/Vocab/Norwegian` and some word tokens
to ignore.
