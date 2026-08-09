---
title: "Brittni's AI Use"
layout: post
author:
  - Brittni Watkins
date: 2026-08-07
modified_date: 2026-08-09
toc: true
read_time: true
description: "How I use AI in my generative (algorithmic) art, my software engineering work, and my writing."
---

## Art and Code and Where They Meet

My work lives at the intersection of art and technology: writing code, something that is typically considered a purely technical skill, becomes a creative process because the code I write creates art.
Navigating the new and evolving landscape of artificial intelligence (AI) has become a challenge in my work, as the technical sphere, where AI use may be more accepted, is completely intertwined with the creative sphere, where AI use is more controversial.
My personal views on AI are nuanced, and as a result I have a very specific approach to how I use AI in my work.

## Do You Use AI to Create Your Generative Art?

I do not use generative AI to create my art.
When I say that I make "generative art", I am saying that I create art *generated* by following a system of rules.
I create and execute those rules using code, but generative art can be created using any medium, including paint, sculpture, music, and poetry.
The history of generative art is rich and complex; it existed long before the advent of AI and even long before the advent of computers.

To reduce confusion, I will sometimes refer to my work as "algorithmic art", rather than "generative art", but the process is the same regardless of the terminology.
I write the code that defines the system, and the computer executes that code to produce an output by following the rules of that system.
Typically, this is achieved through pseudorandom number generation, which allows for a wide range of outputs to be produced from a single set of rules.
My algorithms are hand-coded, meaning that I write every line of code myself; I am not prompting a large language model (LLM) to generate code for me, nor am I using an LLM to generate the art itself.

I do use AI to review my code, including my art code, but the creative decisions and the code that expresses them are mine.
The following sections detail how I use AI in my review process, and how I strive to maintain transparency and accountability in my work.

## Do You Use AI in Your Engineering Work?

I do use AI in my work as a software engineer, but I try to be very intentional and mindful about how and when I use it.
I do not allow AI agents to work autonomously in my repositories.
I use AI primarily in a review capacity, to analyze code I have already written and suggest changes.
I do not use AI tools to author features, refactor across my codebase, or open pull requests, and nothing is merged or published without my review.

### Code Reviews

Once I finish a major changeset in my codebase, I will request a code review from an AI tool to help me identify potential issues, bugs, or areas for improvement.
The AI tool will provide feedback on my code, and I will review that feedback to determine whether it is valid and useful.
I only accept the changes that I feel are beneficial to the code, and I take care to mark the changes that were suggested by AI so that my process remains clear and transparent.

### AI Instruction Files

I also use AI to help me generate and update AI agent instruction files.
When I use AI tools such as GitHub Copilot or Claude Code, I want them to be fully aware of the context of my project and my preferences as a developer.
I don't want the code reviews to constantly suggest changes that I don't want because they don't align with my coding style or the goals of my project.
Instruction files allow me to provide that context and those preferences to the AI tools, so that they can provide more relevant and useful feedback.
I allow the AI tools to suggest changes to the instruction files as the project and code evolve, but I review those changes and only accept the ones that are needed.

You can see an example of an AI instruction file in [`copilot-instructions.md` from my p5-webpack-typescript-template repository](https://github.com/blwatkins/p5-webpack-typescript-template/blob/main/.github/copilot-instructions.md).

### Portfolio Skills Pages

Additionally, I use AI tools to generate and maintain the portfolio skills pages that document the engineering skills showcased in my work.
The portfolio skills pages are meant to be a record of the technical skills that I have demonstrated in a specific project, generated from the context of the codebase itself and instructions that I provide to the AI tools.
Reviews and updates of the portfolio skills pages have been integrated into my code review process to ensure that the pages are accurate and up to date.
Each portfolio skills page includes evidence links with each claim, providing a direct connection between the listed skill and the file or files in my codebase that demonstrate it.
Being able to quickly and easily generate and update these pages has been a huge time-saver for me, allowing me to focus on the code while still maintaining an accurate technical skills record.

You can see an example of a portfolio skills page on [the GitHub Pages site of my p5-webpack-typescript-template repository](https://blwatkins.github.io/p5-webpack-typescript-template/portfolio-skills.html).

### Code Snippets and Examples

I will occasionally use AI tools to generate a small code snippet, an example algorithm, or a "Hello, World!" program.
However, these are always small, self-contained examples that I am using for educational or exploration purposes.
I take the same care with these examples as I do with examples that I find on the internet or in books: I review them, test them, and modify them as needed to ensure that they are correct and useful.
Any code that I choose to include in my codebase is integrated by hand so that I may apply my own coding style and preferences to the code; this also ensures that I am fully aware of how the code works and how it fits into the larger system.

## Do You Use AI in Your Writing?

Whenever I write a blog post or an article, I always write the first draft on my own.
I will occasionally accept sentence and phrase completion suggestions from the autocomplete feature of my code editor, but I do not use AI to generate drafts or outlines for my writing.
I strive to ensure that my writing is my own, and that it reflects my own thoughts, ideas, and voice.
After my first draft is complete, I will ask AI tools to review my writing and provide feedback on grammar, spelling, clarity, and style; I will review the feedback and implement any changes that I feel are necessary or beneficial to the piece.
I wrote this section, for example, after I asked Claude to review this article and it suggested that I add a section about my prose writing in addition to my code and art.

## Transparency and Accountability

Every line of code and every line of text in everything I create is reviewed and approved by me.
I am never blindly accepting changes suggested by AI tools, and I take great care to ensure that AI is not affecting the quality, integrity, or originality of my work.
Additionally, all of my code, including the AI instruction files, is open-source and publicly available in my repositories on GitHub.
All of my code changes are tracked and documented in my GitHub commit history, and I mark which commits I make due to an AI review suggestion in my commit messages.
You can see an example of this in my [p5-webpack-typescript-template repository commit history](https://github.com/blwatkins/p5-webpack-typescript-template/commits/main/), where I have marked the commits that were made due to AI review suggestions with the commit message prefix "Claude Code review:" or "GitHub Copilot review:".

## Closing Thoughts

The use of AI in any creative process has become a hotly debated topic, and I understand that there are many different opinions on the matter.
I do not use AI to create my art, but I do use AI to assist me in my work as a software engineer and a writer.
I know that for some, this will call into question the originality of my work, and may draw criticism or scrutiny about how much of my work is my own and how much is the result of AI assistance.
That being said, I love creating art with code.
I love the work that I do and the things that I create.
The images, experiences, and programs that I make are the bounty of years of study, practice, success, failure, and experimentation.
Each algorithm I publish is the result of weeks and months of research, development, coding, testing, iteration, improvement, and refinement.
My transparency may not be enough for everyone, but I am happy with the approach I have taken, the workflows I have created for myself, and the time, care, and love I put into my code and art every day.

There is beauty in code, and code can make beautiful things.

## Resources and References

For additional information about the concepts mentioned in this article, the following resources may be helpful:

- [Wikipedia - Generative art](https://en.wikipedia.org/wiki/Generative_art)
- [Wikipedia - Algorithmic art](https://en.wikipedia.org/wiki/Algorithmic_art)
- [Claude Code](https://claude.com/product/claude-code)
- [GitHub Copilot](https://github.com/features/copilot)

<footer class="ai-disclaimer">
  <small>This article was written and edited by Brittni Watkins. The AI tools Claude and Claude Code were used for review and feedback.</small>
</footer>
