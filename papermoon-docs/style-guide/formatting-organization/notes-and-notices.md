---
title: Notes and Notices
description: TODO
---

# Notes and Notices

## Introduction

Technical writers will sometimes use notices to offset information that doesn't fit the flow of the text but, the user could still find important or useful. You will hear the team refer to these notices or call-outs as [admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#admonitions){target=\_blank} in alignment with the naming conventions used by Material for Mkdocs.

This style guide divides admonitions into two types:

- **Messaging** - admonitions intended to share a piece of information with the user
- **Layout** - admonitions intended to visually organize and guide the user through technical information such as interfaces, functions, request/response details, and similar items found on a reference style page

## Use Messaging Admonitions

There are a few key things to keep in mind when using messaging admonitions. This section guides you through selecting the best admonition for your use case and customizing the admonition title.

### Select an Admonition

The following messaging admonition types are available across all projects unless otherwise indicated. Select a title to view an example of default styling for that admonition type.

- [**Tip**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#+type:tip){target=\_blank} - optional information that is useful but not critical to help a user be more successful. Users should be able to succeed in a task even if they ignore this information 

- [**Note**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#+type:note){target=\_blank} - highlights information the user should know, even if they are just skimming. Should be a key concept or main idea the page is intending to communicate

- [**Warning**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#+type:warning){target=\_blank} - applied in instances where the user might suffer financial loss, lost data, or a potential security breach if they don't have this information

### Handle Cross-References

Do not use admonitions to create a [cross-reference](https://developers.google.com/style/cross-references){target=\_blank} to another documentation page, repository, or outside resource. For guidance about handling cross-references, see the [Cross References](/papermoon-mkdocs/style-guide/linking/cross-references/) documentation.

### Customize Admonition Title

You have a few options when it comes to the title displayed above your admonition message. This section covers those options and how to apply each one to customize an admonition. Select a title to view an example of the styling for that title option.

- [**Default title**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#usage){target=\_blank} - admonitions will default to using the type qualifier (`tip`, `note`, or `warning`) in titlecase. No additional syntax is needed to use the default title. An example using the default title for the tip admition might look as follows:

    ``` markdown
    !!! tip 

        Lorem ipsum dolor sit amet, IOTA cut off a hot wallet, but Golem allowed a robust volume although ERC20 token standard returns lots of ledger. Since Cardano detected some automated arbitrage in the pump and dump, it built few dormant dolphin.
    ```

- [**Custom title**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#changing-the-title){target=\_blank} - add a quoted string containing valid markdown after the type qualifier to create a custom title for your admonition. The following example updates the `tip` admonition with a custom title:

    ``` markdown
    !!! tip "Basic Attention Token based on few"

        Lorem ipsum dolor sit amet, IOTA cut off a hot wallet, but Golem allowed a robust volume although ERC20 token standard returns lots of ledger. Since Cardano detected some automated arbitrage in the pump and dump, it built few dormant dolphin.
    ```

    If you feel the need for a custom admonition title, make sure you've considered whether adding a heading and copy to the body of your page would be a better way to communicate the message.

- [**No title**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#removing-the-title){target=\_blank} - add an empty string after the type qualifier to omit the title and icon completely. This option should rarely be used when creating messaging admonitions. The following example updates the `tip` admonition to remove the title:

    ``` markdown
    !!! tip ""

        Lorem ipsum dolor sit amet, IOTA cut off a hot wallet, but Golem allowed a robust volume although ERC20 token standard returns lots of ledger. Since Cardano detected some automated arbitrage in the pump and dump, it built few dormant dolphin.
    ```

## Use Layout Admonitions

Guidance for layout admonition usage is currently under development. The team is researching options for programatically generating SDK reference material from their code repositories.  

### Select an Admonition

The following layout admonition types are available across all projects unless otherwise indicated. 

- **Code** - use as an expandable container to share a complete script at the end of a tutorial section. See the [Add Smart Contracts](https://docs.moonbeam.network/tutorials/eth-api/hardhat-start-to-end/#add-smart-contracts){target=\_blank} section of this Moonbeam Hardhat tutorial to see examples of this admonition in use. The following example demonstrates syntax for using the `code` admonition:

    ```markdown
    ??? code "DelegationDAO.sol"
        ```solidity
        INSERT_CODE_SNIPPET_HERE using --8< 'path/to/snippet'
        ```
    ```

    - The `code` admonition should be collapsed by default
    - The title should be the name of the file inside the admonition
    - Limit use to instances where you are sharing the full code of a script or smart contract you previously pretended in pieces, such as the end of a section in a tutorial
    - The `code` admonition is not part of the default supported set and must be configured for each project. If you are using `code` and not getting expected results, please see a member of the formatting team


## Additional Resources

- [**Admonitions**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/){target=\_blank} page - Material for Mkdocs
- [**placehodler**](https://placehodler.shapelabs.co/){target=\_blank} - a crypto themed lorem ipsum generator


