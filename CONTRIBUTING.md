# Contributing

Thank you for your interest in contributing to **awesome-opensource-projects**!


## 2. JSON Structure

Each project lives in its own JSON file:

```text
projects/<category>/<project_name>.json
```

Where `<category>` is one of the existing categories, for example:

- `terminal-cli`
- `web-applications`
- `web-frameworks`
- `devops`
- `operating-systems`
- `management`
- `package-management`
- `testing`
- `text-processing`
- `vpn`

### Required fields

```json
{
  "name": "Project Name",
  "url": "https://github.com/owner/repo-or-external-url",
  "description": "Short one-line description of the project",
  "tech_stack": ["Go", "PostgreSQL", "React"],
  "status": "Active",
  "category": "terminal-cli"
}
```

### Optional fields

```json
{
  "contribution": "Open for contributors",
  "links": {
    "GitHub": "https://github.com/owner/repo",
    "Website": "https://example.com",
    "Docs": "https://docs.example.com"
  }
}
```

---

## 3. Regenerating the README Locally

1. Make sure you have Python 3 installed.
2. From the repository root, run:

   ```bash
   python scripts/generate_readme.py
   ```

3. Open `README.md` and verify that:

   - Your project appears in the correct category
   - The description and links look correct
   - For GitHub projects, badges are shown
   - For non‑GitHub projects, there are no GitHub badges

---

## 4. Opening a Pull Request

1. Fork this repository.
2. Create a new branch:

   ```bash
   git checkout -b add-my-project
   ```

3. Add your JSON file under `projects/<category>/<project_name>`.
4. Run the README generator:

   ```bash
   python scripts/generate_readme.py
   ```

5. Commit and push:

   ```bash
   git add projects/**/*.json README.md
   git commit -m "Add <Project Name> to <Category>"
   git push origin add-my-project
   ```

6. Open a Pull Request and briefly describe your project and chosen category.


## Join the Open Source Community

This list is maintained by the **Опенсорсеры** (Open Source Developers) community.

If you want to:

- discuss open source projects,
- find collaborators,
- get feedback on your own project,

join us on Telegram:

<a href="https://t.me/OpenSource_Chat">
    <img src='assets/join.svg'/>
</a>
