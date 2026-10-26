# Week 1 Linux Hands-on Lab: Your First Project Workspace

This lab practices Linux directories, files, file searches, and process IDs.

## Folder structure

```text
week1/
├── README.md
├── scripts/
│   └── notes.txt
└── screenshots/
    ├── 01-create-workspace.png
    ├── 02-create-notes.png
    ├── 04-create-scripts.png
    ├── 05-move-notes.png
    ├── 06-find-notes.png
    └── 07-identify-process.png
```

## Tasks and commands

The screenshots below are the original supplied evidence. The project is stored
in this repository's `week1/` folder. The first screenshot shows the requested
`~/cloud-devops/week1` command; subsequent screenshots show work inside the
`Cloud-Devops/week1` repository directory.

| Task | Command | Evidence |
| --- | --- | --- |
| 1. Create the workspace | `mkdir ~/cloud-devops/week1` | [Screenshot](screenshots/01-create-workspace.png) |
| 2. Create notes.txt | `touch notes.txt` | [Screenshot](screenshots/02-create-notes.png) |
| 3. Add text to notes.txt | See command below | [Completed notes](scripts/notes.txt); screenshot still needed |
| 4. Create scripts directory | `mkdir scripts` | [Screenshot](screenshots/04-create-scripts.png) |
| 5. Move notes into scripts | `mv notes.txt scripts/` | [Screenshot](screenshots/05-move-notes.png) |
| 6. Search for notes.txt | `find . -name "notes.txt"` | [Screenshot](screenshots/06-find-notes.png) |
| 7. Identify a running process and PID | `ps` | [Screenshot](screenshots/07-identify-process.png) |

To reproduce the text addition after moving the file, run this from `week1/`:

```bash
printf '%s\n' \
  'Week 1 Linux Hands-on Lab: Your First Project Workspace' \
  'I practiced creating directories and files, writing text, moving files,' \
  'searching for files with find, and identifying process IDs with ps.' \
  > scripts/notes.txt
cat scripts/notes.txt
```

The file search returned `./scripts/notes.txt`. In the supplied `ps` screenshot,
`bash` had PID **196631**, and `ps` had PID **207879**. These are historical
values from that terminal session; process IDs change between sessions.

## GitHub submission

Repository: [AbdulazizAyalew/Cloud-Devops](https://github.com/AbdulazizAyalew/Cloud-Devops)

The existing local repository is connected through its `origin` remote:

```bash
git remote -v
git add README.md week1/
git commit -m "Document Week 1 Linux lab and organize screenshot evidence"
git push origin main
```

## Remaining submission steps

- Capture a screenshot showing the text-addition command and `cat scripts/notes.txt`
  output, then save it as `screenshots/03-add-text.png` and commit and push it.
- Submit the repository link in the Week 1 section of the Cloud & DevOps track sheet.

Six original screenshots are included. Task 3's file is completed, but its screenshot
was not supplied. The track sheet submission has not been performed here.
