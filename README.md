# devonfw Getting Started Guide

![devonfw logo](theme/images/devonfw-small.png "Welcome, new devonfw user!")

Welcome!

This getting-started guide is the entry-point for new **devonfw** users.\
You can work through it by either visiting the [wiki](https://github.com/devonfw/getting-started/wiki) tab here on GitHub or by downloading the [PDF](https://github.com/devonfw/getting-started/raw/master/devonfw_getting_started.pdf).

Happy coding! :thumbsup:

---

## How to maintain this guide

Please follow these guidelines when maintaining the *getting-started* repository:

- Use links and references instead of duplicating content from other repositories!

- Always keep the contents of `_Sidebar.asciidoc` and `master-getting-started.asciidoc` in sync!

- In the **_Sidebar**:

  - link AsciiDoc pages located in this repo via `link:asciidoc-file-name.asciidoc[link title]`\
  (Please make sure to include the `.asciidoc` file extension here!)

  - link external pages via `https://online-url.domain#anchor[link title]`

- In **master-getting-started**:

  - include AsciiDoc pages located in this repo via `include::file-name[leveloffset=2]`\
  (Please make sure to omit the `.asciidoc` file extension here!)

  - reference AsciiDoc sections via `xref:section-title[link title]`

  - reference AsciiDoc pages and top-level sections via `link:file-name#section-title[link title]`\
  (Please note, that these links will **NOT** work in the GitHub wiki and standalone PDF, if the linked files are not located in this repo. They will however work on the devonfw website and in the complete devonfw-guide PDF, which is our priority.)

- Follow the general [docgen guidelines](https://github.com/devonfw/docgen/wiki#guidelines) and [asciidoc file guidelines](https://github.com/devonfw/devonfw-guide/issues/43)

- To test your changes, build a local PDF using Maven: `mvn clean package -Doutput.format=pdf`