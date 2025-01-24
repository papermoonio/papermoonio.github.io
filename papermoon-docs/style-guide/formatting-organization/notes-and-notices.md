---
title: Notes and Notices
description: Learn how to master different types of admonitions in MkDocs to improve clarity, organization, and UX for better content creation.
---

# Notes and Notices

## Introduction

Technical writers sometimes use notices to offset information that doesn't fit the flow of the text, but the user can still find it necessary or valuable. You will hear the team refer to these notices or call-outs as [admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#admonitions){target=\_blank} in alignment with the naming conventions used by Material for Mkdocs.

This style guide divides admonitions into two types:

- **Messaging** - admonitions intended to share a piece of information with the user
- **Layout** - admonitions intended to visually organize and guide the user through technical information such as interfaces, functions, request/response details, and similar items found on a reference style page

## Use Messaging Admonitions

There are a few key things to remembere when using messaging admonitions. This section guides you through selecting the best admonition for your use case and customizing the admonition title.

### Select an Admonition

The following messaging admonition types are available across all projects unless otherwise indicated. Select a title to view an example of default styling for that admonition type.

- [**Tip**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#+type:tip){target=\_blank} - optional information that is useful to help a user be more successful but not critical. Users should be able to succeed in a task even if they ignore this information 

- [**Note**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#+type:note){target=\_blank} - highlights information the user should know, even if they are skimming. Should be a key concept or main idea the page is intending to communicate

- [**Warning**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#+type:warning){target=\_blank} - applied in instances where the user might suffer financial loss, lost data, or a potential security breach if they don't have this information

### Handle Cross-References

Do not use admonitions to create a [cross-reference](https://developers.google.com/style/cross-references){target=\_blank} to another documentation page, repository, or outside resource. See the [Cross References](/papermoon-mkdocs/style-guide/linking/cross-references/){target=\_blank} documentation for cross-referencing guidance.

### Customize Admonition Title

You have options regarding the title displayed above your admonition message. This section covers how to change the title to customize an admonition. Select a title to view an example of the styling for that title option.

- [**Default title**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#usage){target=\_blank} - admonitions will default to using the type qualifier (`tip`, `note`, or `warning`) in titlecase. No additional syntax is needed to use the default title. An example using the default title for the tip admonition might look as follows:

    ``` markdown
    !!! tip 

        Lorem ipsum dolor sit amet, IOTA cut off a hot wallet, but Golem allowed a robust volume although ERC20 token standard returns lots of ledger. Since Cardano detected some automated arbitrage in the pump and dump, it built few dormant dolphin.
    ```

- [**Custom title**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#changing-the-title){target=\_blank} - add a quoted string containing valid markdown after the type qualifier to create a custom title for your admonition. The following example updates the `tip` admonition with a custom title:

    ``` markdown
    !!! tip "Basic attention token based on few"

        Lorem ipsum dolor sit amet, IOTA cut off a hot wallet, but Golem allowed a robust volume although ERC20 token standard returns lots of ledger. Since Cardano detected some automated arbitrage in the pump and dump, it built few dormant dolphin.
    ```

    If you need a custom admonition title, considered whether adding a heading and copy to the body of your page would be a better way to communicate the message. Custom admonition titles should use sentence case.

## Use Layout Admonitions

Guidance for using layout admonitions is currently being developed. The team is also researching options for programmatically generating SDK reference material from their code repositories.  

### Select an Admonition

The following layout admonition types are available across all projects unless otherwise indicated. 

- **Code** - use as an expandable container to share a complete script at the end of a tutorial section. See the [Add Smart Contracts](https://docs.moonbeam.network/tutorials/eth-api/hardhat-start-to-end/#add-smart-contracts){target=\_blank} section of this Moonbeam Hardhat tutorial to see examples of this admonition in use. The following example demonstrates the syntax for using the `code` admonition:

    ```markdown
    ??? code "DelegationDAO.sol"
        ```solidity
        INSERT_CODE_SNIPPET_HERE using --8< 'path/to/snippet'
        ```
    ```

    - The `code` admonition should be collapsed by default
    - The title should be the name of the file inside the admonition
    - Limit use to instances where you are sharing the complete code of a script or smart contract you previously presented in pieces, such as the end of a section in a tutorial
    - The `code` admonition is not part of the default supported set and must be configured for each project. If you are using `code` and not getting the expected results, please see a member of the formatting team

## Additional Resources

- [**Admonitions**](https://squidfunk.github.io/mkdocs-material/reference/admonitions/){target=\_blank} page - Material for MkDocs
- [**placehodler**](https://placehodler.shapelabs.co/){target=\_blank} - a crypto themed lorem ipsum generator


