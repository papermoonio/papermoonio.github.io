---
title: Learn Pages
description: TODO
---

# Wormhole Learn Pages

## Introduction

The Wormhole Docs use Learn as the section for informational content. Learn pages are structured to implement the [Explanation](https://diataxis.fr/explanation/){target=\_blank} Diataxis documentation form and the [Concept](https://www.thegooddocsproject.dev/template/concept){target=\_blank} The Good Docs Project content type. The following sections use concept to refer to the topic or idea your content is about.

## Purpose of Learn Pages

The primary purpose of Learn pages is to develop the user's understanding of the concept. Consider the following guidelines when planning a Learn page:

:white_check_mark: Provide clear, concise, and consistent information about a specific concept or process

:white_check_mark: Give the user context that will help in understanding the more specific content ahead

:white_check_mark: Explain the context and components of a tool or product and how they fit into the broader framework

:x: Do not include how-to steps or reference information in the body copy

## Before You Start Writing

The single most important thing you can do before you start writing is to think about the target audience and what they might need from this page. The following sections contain additional activities you may find useful during the planning phase. 

### Map Out the Concept

Use a sketch, diagram, or outline to help you to organize the information in your mind and see the entire concept at once. Possible questions to answer during this step include:

- How does the concept connect to other concepts?
- Where does it fit in the broader ecosystem?
- What dependencies exist? Are there concepts a user should know before they read this content?

If you do this part well, you may come away with the start of a nice diagram or visual aid for your page.

### Collect User Feedback 

User feedback can be a powerful tool in shaping documentation to best meet user needs. Collect common questions or concerns where possible and use them to guide your content development. Possible sources of feedback might include:

- Submissions to the feedback widget
- Hackathon participant feedback
- GitHub issues on project repositories
- Developer discussions in places like Discord and Telegram

### Organize Information

Use the inverted pyramid structure to organize Learn page information. With the inverted pyramid, the information the user most needs to know is presented first. The rest of the information is ordered from most important to least important. 

The [Inverted pyramid structure](https://www.stylemanual.gov.au/structuring-content/types-structure/inverted-pyramid-structure){target=\_blank} page from the Australian Government Style Manual provides a deeper look at effective use of the inverted pyramid.

## Name a Learn Page

The title of a Learn page is your first opportunity to help the user identify the topic of the page. Consider the following guidelines and options when naming a Learn page:

- **Name of concept** - use the name of the concept as a noun

    :white_check_mark: Token Bridge, Core Contracts, and similar

- **Overview** - overview page titles should typically include the topic or concept

    :white_check_mark: Overview of Transfer Protocols

    :white_check_mark: Transfer Protocol Overview

    :x: Avoid using Overview by itself as a page title

- **Introduction** - introduction page titles should typically include the topic or concept

    :white_check_mark: Introduction to Wormhole

    :white_check_mark: Introduction to Multichain Applications

    :x: Introduction

- **Meta title** - each Learn page must include an SEO-friendly meta title of between 34 and 44 characters

    :white_check_mark: The meta title combined with "| Womrhole Docs" should total between 50 and 60 characters 

    :white_check_mark: The title in the left navigation and the title rendered on the page can be different

If you have a title you would like to use that doesn't fit these guidelines, please discuss it with the formatting team prior to opening your pull request. 

## Create Learn Page Description

Each Learn page must include an an SEO-friendly meta-description of between 120 and 160 characters. You can use Grammarly as an assistant for this task by following these steps:

1. Paste your copy into a Grammarly document
2. Select the **Write with generative AI** tab at the top of the right-hand column
3. Use a prompt similar to the following:

    ```text
    Please create an SEO-friendly description between 120 and 160 characters for this page
    ```

4. Make any needed adjustments to the generated text and add it to the description field of your document

## Style Guidance

All Wormhole Learn pages should include the following:

- **SEO-friendly meta title** - between 34 and 44 characters. This title plus the copy "| Wormhole Docs" should equal 50 to 60 characters in total
- **SEO-friendly meta description** - between 120 and 160 characters
- **H1 heading page title** - this is the title that will render at the top of the page and may be different than the meta title
- **Content or body text** - all Learn pages should increase the user's understanding of the concept and provide needed context for the more specific content they will eventually encounter. The following elements contribute to a quality Learn page:
    
### Introduction 

Your opening paragraph should immediately tell the user if this page is of interest or use to them. Consider the following guidance when writing the first paragraph of the introduction:

- Introduce the concept. What is it?
- Provide context. Why is it important or relevant? 
- Preview upcoming content. What will the user find here?

Examples - see the following for examples of quality opening paragraphs:

- [Introduction to the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction){target=\_blank} page of MDN 
- [Core Contracts]({target=\_blank}){target=\_blank} page of Wormhole Docs

Following the opening paragraph, add one to two paragraphs to address the following points where relevant:

- **Functionality** - what does the product or concept do?
- **Define the Concept** - think of a glossary definition. The goal is to create a shared understanding of the concept between the writer and reader
- **The Big Picture** - explain how this concept fits into the bigger picture of products or concepts. Focus language on the problem solved and benefits of the solution 
- **Key Features** - a bullet list of key features can be helpful here
- **Visual Aid or Diagram** (optional) - use if it will help illustrate how the concept is organized or how it fits into the broader system or product

Example - see the following for an example of defining a concept:

- [Processor](https://cloud.google.com/document-ai/docs/overview#dai-processors){target=\_blank} section of the Google Cloud Document AI documentation

### Use Cases

This is a great opportunity to link users to future steps in the developer journey. Depending on the overall length of the Learn page, use paragraphs or bullet lists to briefly share use cases related to the concept or product. A quality use case will include a brief explanation of the problem being solved and specifically how the presented concept solves the problem.

Example - see the following for an example of defining use cases:

- [Document AI components](https://cloud.google.com/document-ai/docs/overview#components){target=\_blank} section of the Google Cloud Document AI documentation

### Comparison Section (optional)

Use this section to include a comparison table, or link to one elsewhere on the site, if appropriate. 

### How It Works

Includes one to two paragraphs to briefly explain how the concept operates and the main components involved in any associated process. This is where you can go into more detail for those who have read this far down the page. 

### Related Resources 

Create a bulleted list of links to informational resources related to the page contents or relevant Reference page entries. 

### Where to Go Next

Create a bulleted list of guides and tutorials related to the page contents to guide the developer journey toward using what they learned.

## Learn Page Template

--8<-- 'code/style-guide/key-resources/templates/wormhole/index-pages/wh-learn-template.md'

## PR Checklist

Before requesting PR review, please ensure you have:

1. Used Grammarly to review your work and made edits as needed
2. Served the site locally for a visual review of rendering and made updates as needed

    You can serve the site locally by running the following command from the `wormhole-mkdocs` directory:

    ```bash
    mkdocs serve
    ```

3. Checked the PR checklist on GitHub and completed any items listed there

## Addtional Resources

- [**Character Counter**](https://wordcounter.net/character-count){target=\_blank} - quickly check the character length of your titles and descriptions
- [**Title Case Converter**](https://titlecaseconverter.com/){target=\_blank} - verify title case for titles or headlines