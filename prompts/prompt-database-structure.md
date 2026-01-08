Create a suggested database markdown file in DBML format, put it in the `@docs/database-schema.md` file. It should follow the requirements for the `@docs/user-stories.md` and `@docs/project-description.md`.

Follow best practices and typical convensions for Laravel 12 databases.

---

## Guidelines for Laravel DB

- Don't use Enum DB fields, unless absolutely sure the values won't change. For values that would rarely change, create string DB value with a comment of first values, so that PHP Enum is expected in the future. For values that would change more often, create lookup tables with foreign keys.
- Don't create new DB tables that may conflict with same name as existing default Laravel DB tables, like "users" or "jobs".
- For file/image uploads, use the package `spatie/laravel-medialibrary` with DB table `media` coming from that package, unless instructed otherwise.
