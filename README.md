# File Manager App

This is an ai coding experiment repo. In it, I'm using [Zed](https://zed.dev/) with [Claude Opus 4](https://www.anthropic.com/claude/opus) as the ai assistant. The major goal of this project is to explore a development worklfow using driving the code writing tasks.

As this is more of a research project, the `./docs` directory is a [logseq](https://logseq.com/) graph for my notes, ideas, documentation of prompts and variations, and critiques.

## Install Instructions
- Install Dependencies:  `npm i` in the `./src` directory
- Start development server: `npm run dev`
- View Documentation: Open `./docs` in logseq (or view the files however, it's mostly markdown)

## Project Outline
- **Objective**: Build a file management app that features a GUI and manages files in a sql database
- **Purpose**: Experiment with using AI as the main code writer in a project and to document my findings of what works well vs what causes more issues.
- **Target Audience**: Other developers and learners most likely, myself. This isn't really intended to have an actual user base
- **Timeline**: 5 days casual
  - Day 1: Scaffold app with production and development pipelines (Frontend, Backend, Database). also set up linter and formatter
  - Day 2: Configure user tables in the DB and connect to backend, basic security and environment variables
  - Day 3: Backend commands and communication with DB, CRUD operations should be complete
  - Day 4: build frontend using [htmx](https://htmx.org/) and vanilla css
  - Day 5: Test out on mobile and desktop
- **Scope**:
  - A user can create an account with email and password
  - The user gets 2 gb of data storage
  - The user can reset their password (must answer questions, simple and not secure but no email server)
  - No email confirmation (not setting up an email server at this time)
  - User account can:
    - View files in a table
    - Add files
    - Delete files (permanent and send to trash)
    - Edit file name
    - Download file
    - Give themself a user name that they can then sign in with
  - UI is to be fairly minimal and clean (not a major priority)
    - responsive css using media queries, flexbox, and grid consistently
    - interactions should feel natural and easy
    - clear visual feedback
- **What I want to get out of this**
  - to develop my AI coding skills so I can have an informed opinion and practical experience
  - to also experiment with a project based logseq graph. I want to see how well this works for me, especially for research repos
  - to get better at coding
  - to challenge my assumptions and current knowledge
  - to consider and document how [Systems Thinking](https://en.wikipedia.org/wiki/Systems_thinking) is relevant to this process -- document and ideate

## MVP User Stories
- As a user, I can sign up to the app (simulated on my computer in a podman pod)
- As a user, I can upload, download, and edit filenames of files in my 2gb file storage space
- As a user, I can view all the files and information about them (last accessed, size, name, type)
- As a user, I can create folders for grouping my files
- As a user, I can delete files and folders
- As a user, I can change filenames of files and folders
