These permissions are shown utilizing the `octal` or Base 8 numbering system. They are used to apply the `read`, `write`, and `execute` attributes to the contexts of `User owner`, `Group owner`, and `Others` on a file. These are represented as:

| **Attribute**   | **Octal Value**    |
| --------------- | ------------------ |
| (`r`) - Read    | `Octal value of 4` |
| (`w`) - Write   | `Octal value of 2` |
| (`x`) - Execute | `Octal value of 1` |

        shellsession
`malvvare@htb[/htb]$ ls -l   - rw- r-- r--@  1 htb-user staff 2512910 Aug 30  2019 HTB-Wallpaper-1.png - |_| |_| |_|   |    |       |     |      |_______| |  |   |   |    |    |       |     |          |__ Date |  |   |   |    |    |       |     |_____________ File Size |  |   |   |    |    |       |___________________ Group |  |   |   |    |    |___________________________ User |  |   |   |    |________________________________ Number of hard links |  |   |   |___ Permissions of others (everyone else)(read) |  |   |_______ Permissions of the group (staff)(read) |  |___________ Permissions of the User owner (htb-user)(read, write) |______________ File type (- = File, d = Directory, l = Link, ... )`