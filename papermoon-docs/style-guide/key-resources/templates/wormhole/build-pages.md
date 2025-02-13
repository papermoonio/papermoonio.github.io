---
title: Build Pages
description: TODO
---

# Wormhole Build Pages

## Introduction

The Wormhole Docs use Build as the section for how-to guide related content. Build pages are structured to implement the [How-to guide](https://diataxis.fr/how-to-guides/){target=\_blank} Diataxis documentation form and the [How-to guide](https://www.thegooddocsproject.dev/template/how-to){target=\_blank} The Good Docs Project content type. The following sections use tasks to refer to the objective the user wants to achieve by using the how-to guide.

## Purpose of Build Pages

The primary purpose of Build pages is to help the user solve a real-world problem or complete a task. Consider the following guidelines when planning a Build page:

:white_check_mark: Take the user through a series of steps for the surest and safest way to solve a problem, complete a task, or troubleshoot an issue

:white_check_mark: Clearly and concisely describe a set of sequential steps the user must complete to accomplish the goal

:white_check_mark: Build page how-to guides assume the user has basic knowledge of blockchain development and Wormhole concepts

:white_check_mark: Alert the user to possible issues or difficulties and provide guidance on resolving them

:x: Do not include concept explanation or reference information in the body copy

## Before You Start Writing

The most important thing you can do before you start writing is to think about the target audience and what they might need from this page. The following sections contain additional activities you may find useful during the planning phase.

### Identify Scenarios

Once you identify the task the Build page will cover, it is helpful to consider different scenarios your user may encounter when carrying out the task in the real world. The best way to do this is to walk through the task yourself. Make sure you've completed the task and understand the places where a user might have questions or decision points requiring guidance. 

### Map the Safest Path

There is often more than one possible way to complete a task. Your goal as the creator of the Build page is to map out the safest, surest path to completing the task. Suggesting multiple ways to complete a task asks the user to analyze those options, understand them, and determine which option will best solve their problem. Make their journey easier and provide a reliable path to accomplishing the task. 

### Anticipate Error Scenarios

Track any errors you encounter while working through the task and identify scenarios. Your Build page should include troubleshooting information anywhere you anticipate the user may encounter errors.

## Name a Build Page

The title of a Build page should tell the user what task they can accomplish by following the guide. Consider the following guidelines and options when naming a Build page:

- **Use a Verb** - start the title with the plain, or base, form of a verb such as "Build," "Integrate," or "Configure"

    :white_check_mark: Send Messages with Wormhole Relayer

    :white_check_mark: Interact with CCTP Contracts

- **Avoid Use of Present Participles** - also known as gerunds, the "-ing" form of verbs makes content more challenging to translate and, therefore, decreases accessibility

    :x: Building Cross-Chain Applications

    :x: Integrating Smart Contracts

- **Communicate the Task** - the page title should tell the user what the guide will help them accomplish as completely as possible

    :white_check_mark: Run a Custom Relayer

    :white_check_mark: Upgrade Contracts

    :x: Deployment

- **Meta title** - each Learn page must include an SEO-friendly meta title of between 34 and 44 characters

    :white_check_mark: The meta title combined with "| Womrhole Docs" should total between 50 and 60 characters 

    :white_check_mark: The title in the left navigation and the title rendered on the page can be different

If you have a title you would like to use that doesn't fit these guidelines, please discuss it with the formatting team before opening your pull request. 

## Create Build Page Description

Each Build page must include an SEO-friendly meta-description of between 120 and 160 characters. You can use Grammarly as an assistant for this task by following these steps:

1. Paste your copy into a Grammarly document
2. Select the **Write with generative AI** tab at the top of the right-hand column
3. Use a prompt similar to the following:

    ```text
    Please create an SEO-friendly description between 120 and 160 characters for this page
    ```

4. Make any needed adjustments to the generated text and add it to the description field of your document

## Name a Subtask

As you name the subtasks within your Build page to create section headings, consider the following guidelines:

- **Consider SEO** - keep these headings informative to improve SEO performance, discoverability, and accessibility

- **Use a Verb** - similar to the page title, headings should use plain or base forms of verbs

- **Create an Outline** - create an outline using just the headings for the subtasks and review it to ensure the user can readily determine the upcoming activities using the headings alone

## Style Guidance

All Wormhole Build pages should include the following:

- **SEO-friendly meta title** - between 34 and 44 characters. This title plus the copy "| Wormhole Docs" should equal 50 to 60 characters in total
- **SEO-friendly meta description** - between 120 and 160 characters
- **H1 heading page title** - this is the title that will render at the top of the page and may be different than the meta title
- **Content or body text** - all Build pages should help the user solve a real-world problem or complete a task. The following elements contribute to a quality Build page:
    
### Introduction 

Your opening paragraph should include the following: 

- a clear description of the task completed in the guide 
- when and why the user might want to perform the task

Example - see the [introduction](https://docs.stripe.com/no-code/subscriptions){target=\_blank} from the Create subscriptions page of the Stripe docs

### Prerequisites

The Prerequisites section should include a statement advising the user of which items the Build page assumes they have basic knowledge, including knowledge of fundamental blockchain development and Wormhole concepts. Following this statement, include a bullet list of additional things the user needs to know, install, or have available, which may include items such as the following:

- Specific Wormhole concepts they should know with links to related Learn pages
- Software or hardware requirements
- Environments to set up and configure
- Testnet tokens or wallets
- Authentication and authorization information such as API or private keys

Whenever possible, link the user to a resource that will help them complete a prerequisite, such as outside documentation, relevant Learn pages, or token faucets.

Example - see the following for an example of a quality prerequisites section:

- [Prerequisites](https://wormhole.com/docs/build/contract-integrations/core-contracts/#prerequisites){target=\_blank} section of Get Started with Core Contracts in the Wormhole docs
- [Prequisites](https://docs.polkadot.com/tutorials/polkadot-sdk/parachains/zero-to-hero/obtain-coretime/#prerequisites){target=\_blank} section of Obtain Coretime in the Polkadot docs

### Style Subtasks

For each subtask in the guide, use the heading to list the name of the subtask, followed by a numbered list of steps to follow to complete that task. For each numbered step, include the following:

- **Action to take** - start with a verb 

    :white_check_mark: 1. Create a new folder

- **Explanatory text** - should be minimal and concise 

    :white_check_mark: Use the following commands to create a new folder:

- **Code sample or screenshot** - (optional) add when a visual aide can help the user better understand the step

    :white_check_mark: Include the name of the file by adding `title="filename.extension"` to the top code fence similar to:

    ```text
    ```javascript title="filename.js"
    ```

- **Result** - (optional) where appropriate, tell the user what they can expect if they performed the step correctly

    :white_check_mark: If successful, you will see terminal output similar to the following:

Example - see the following for an example of documenting a subtask:

- [Create a subscription](https://docs.stripe.com/no-code/subscriptions#create-subscriptions){target=\_blank} task in the Stripe docs

### Related Resources 

Create a bulleted list of links to informational resources related to the page contents, such as Learn pages, source code, or relevant Reference page entries. 

### Where to Go Next

Create a bulleted list of guides and tutorials related to the page contents to guide the developer in completing related tasks.

## Build Page Template

--8<-- 'code/style-guide/key-resources/templates/wormhole/index-pages/wh-build-template.md'

## PR Checklist

Before requesting a PR review, please ensure you have completed the following:

1. Used Grammarly to review your work and made edits as needed
2. Served the site locally for a visual review of rendering and made updates as needed

    You can serve the site locally by running the following command from the `wormhole-mkdocs` directory:

    ```bash
    mkdocs serve
    ```

3. Checked the PR checklist on GitHub and completed any items listed there

## Additional Resources

- [**Character Counter**](https://wordcounter.net/character-count){target=\_blank} - quickly check the character length of your titles and descriptions
- [**Title Case Converter**](https://titlecaseconverter.com/){target=\_blank} - verify title case for titles or headlines