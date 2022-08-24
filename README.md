![languagetool-code-comments](.github/banner.jpg)

[![Build Status](https://img.shields.io/github/workflow/status/dustinblackman/languagetool-code-comments/Test?branch=master)](https://github.com/dustinblackman/languagetool-code-comments/actions)
[![Release](https://img.shields.io/github/v/release/dustinblackman/languagetool-code-comments)](https://github.com/dustinblackman/languagetool-code-comments/releases)
[![Coverage Status](https://coveralls.io/repos/github/dustinblackman/languagetool-code-comments/badge.svg?branch=master)](https://coveralls.io/github/dustinblackman/languagetool-code-comments?branch=master)

`languagetool-code-comments` integrates the LanguageTool API to parse, spell check, and correct the grammar of your code comments! Never will you submit a PR where you fat-fingered `// This is a hck` in your code again. LTCC can be integrated directly in your editor, or used in a linting fashion in your CI pipelines. Caching is built in to speed up processing new and edited docs.

Using the power of [Tree Sitter](https://tree-sitter.github.io/tree-sitter/#available-parsers), LTCC easily integrates with several programming languages. And if privacy is a concern, and you have some spare hardware lying around, LanguageTool offers a [great way](https://dev.languagetool.org/http-server) to self-host your own instance.

<!-- command-help start -->
```
languagetool-code-comments 0.1.0
Integrates the LanguageTool API to parse, spell check, and correct the grammar of your code
comments!

USAGE:
    languagetool-code-comments <SUBCOMMAND>

OPTIONS:
    -h, --help       Print help information
    -V, --version    Print version information

SUBCOMMANDS:
    cache         Functionality around the LanguageTools result cache.
    check         Parses source code comments from the provided file and passes them to
                      LanguageTool, returning grammar and spelling mistakes if any.
    completion    Generates shell completions
    help          Print this message or the help of the given subcommand(s)

SUPPORTED LANGUAGES:
  - bash
  - go
  - javascript
  - jsx
  - python
  - rust
  - tsx
  - typescript
```
<!-- command-help end -->
