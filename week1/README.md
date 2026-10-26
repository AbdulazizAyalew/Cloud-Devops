# Week 1 Linux Hands-on Lab

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
    ├── 03-add-text.png
    ├── 03-verify-text.png
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
| 3. Add text to notes.txt | See command below | [Add text](screenshots/03-add-text.png), [verify contents](screenshots/03-verify-text.png), [notes](scripts/notes.txt) |
| 4. Create scripts directory | `mkdir scripts` | [Screenshot](screenshots/04-create-scripts.png) |
| 5. Move notes into scripts | `mv notes.txt scripts/` | [Screenshot](screenshots/05-move-notes.png) |
| 6. Search for notes.txt | `find . -name "notes.txt"` | [Screenshot](screenshots/06-find-notes.png) |
| 7. Identify a running process and PID | `ps` | [Screenshot](screenshots/07-identify-process.png) |

