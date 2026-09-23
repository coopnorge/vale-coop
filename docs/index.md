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

The example above adds a local [vocabulary][Vale vocabularies] that Vale will
look for in `.vale/styles/Vocab/Norwegian`, along with some word tokens to
ignore.

## Vocabulary guide

See [Writing vocabulary entries](vocabularies.md) for guidance on writing one
canonical regex per word, selecting the right shared vocabulary, and creating a
repository-local vocabulary.

[Vale vocabularies]: https://vale.sh/docs/topics/vocab/
