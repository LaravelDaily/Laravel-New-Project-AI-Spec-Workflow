1. **Initial Project Analysis**. Read the job description and think about tech-stack choice and specifically **Starter Kit** for the project installation.

2. **Laravel Installation**. Run `laravel new` with the starter kit chosen in point 1 above. Install Laravel Boost with default Guidelines, for now. If Filament (or other *fundamental architecture* package like `spatie/laravel-medialibrary`) is needed, install it here.

3. **AI Guidelines**. Add custom guidelines to the `.ai/guidelines` folder and run `php artisan boost:install` so it would recognize both Filament and custom guidelines.

4. Install and configure [Context7](https://github.com/upstash/context7), so it would catch the documentation for other Laravel packages and libraries, not available in Laravel Boost, like `spatie/laravel-medialibrary`.

5. **Project Description**. Save the original project description as a file `docs/project-description.md`. If tech-stack is not specified, choose the **tech stack** and add it to the document. Choice of Laravel version, Filament if applicable, Starter Kit, etc. Specify if it's a demo project for education purposes, so AI would suggest smaller scope of features.

6. **User Stories**. Run this [user stories prompt](./prompts/prompt-user-stories.md) in Claude Code or other AI agent of choice. As a result, you should get a new file `docs/user-stories.md`. Review it with AI and/or manually before proceeding.

7. **Database Structure**. Run this [database structure prompt](./prompts/prompt-database-structure.md) in AI agent. As a result, you should get a new file `docs/database-structure.md`. Review it with AI and/or manually before proceeding.

8. **Project Phases**. Run this [project phases prompt](./prompts/prompt-project-phases.md) in AI agent. As a result, you should get a new file `docs/project-phases.md`. Review it with AI and/or manually.

---

At this point, you should have all the files in `@docs` folders, needed to start with the project, prompting AI agent to start with Phase 1 from `@docs/project-phases.md` file.
