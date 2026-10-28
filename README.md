# What to do in the first hour after you delete a file

Short version: **stop writing to that disk.** Every minute you keep using the
machine, the odds go down. The order of the first ten minutes matters more than
which recovery program you eventually buy.

Available in [العربية](README.ar.md) · also on the site in
[Arabic](https://istidaaf.com/) · [English](https://istidaaf.com/en) ·
[Persian](https://istidaaf.com/fa) · [Turkish](https://istidaaf.com/tr).

## Do this

1. Stop saving, downloading and installing. Every new write can land on the
   exact sectors your file used.
2. If the files were on the **system disk**, shut the machine down properly.
   Don't leave the OS paging, indexing and updating on top of them.
3. Note **where** the file was and **how** it disappeared: Recycle Bin /
   Trash, `Shift+Delete`, format, malware, cloud sync conflict. These are very
   different situations with very different odds.
4. Check the easy places first: Recycle Bin / Trash, the cloud web UI
   (OneDrive, Google Drive, iCloud and Dropbox each keep their own trash and
   their own version history, separate from what is on the disk),
   `Previous Versions`, and any backup you forgot about.
5. Photograph or screenshot the folder path. You will want the exact name later.
6. If it is a **phone**, put it in airplane mode. Same reason: stop writes.
7. Write the recovered files to a **different** disk. Recovering onto the same
   disk can overwrite what you are trying to get back.
8. On Linux/macOS, if the drive has to stay mounted, mount it read-only.
9. Set expectations honestly: an SSD with TRIM often means the data is already
   gone. That is a hardware fact, not something a program can fix.
10. Decide *before* you install anything whether the data is worth paying for.

## Don't do this

1. **Don't install the recovery tool onto the disk you lost data from.**
2. Don't run "optimizers", "cleaners" or defragmenters. They write a lot.
3. Don't format, don't run `chkdsk /f`, don't "repair" the partition first.
4. Don't trust a tool that promises 100%. An honest answer is always a range.
5. Don't pay before you know which situation you are in. Some are free to fix
   yourself; some are unrecoverable and no software changes that.

## Four cases, four very different answers

| Situation | What usually survives | Realistic odds |
| --- | --- | --- |
| Recycle Bin emptied / `Shift+Delete`, HDD | File records, often the whole cluster chain | Good, if you stopped writing |
| Recycle Bin emptied, SSD with TRIM | Little: the controller may have zeroed the blocks | Poor |
| Quick format, HDD | Usually just the table; data intact until overwritten | Good |
| Full format / overwritten / bad sectors | Depends; partial recovery only | Low |

These are rough buckets, not a promise. Anything important should come from a
backup, not from recovery.

## A free in-browser check

[RAJ3A](https://istidaaf.com) asks four questions (where the file was, how it
disappeared, what kind of storage, what you have already tried) and returns an
ordered checklist plus an honest probability range.

It runs entirely in your browser: **no file is uploaded and nothing is sent to
a server.** That matters when the thing you lost is private — a tax return, a
medical scan, a client contract.

There is also a paid offline kit, but the triage page is free and does not
require an account.
