# The Long Way Down

## Category
Forensics

## Difficulty
Easy-Medium

## Description  (what players see)
I left it somewhere in this maze of folders.
I don't remember which room I put it in,
only that I walked a long, long way to get there.

## Topics
- File and directory traversal
- Scripting (find / awk / Python / PowerShell)
- Hex <-> ASCII encoding

## Hosting information
Attach trailhead.zip to the challenge for players to download.
Do NOT attach the writeup.
Tell players to extract it somewhere with a SHORT path (e.g. C:\ctf\ or ~/ctf/),
because the deepest folder path is ~110 characters.

## Flag
foobarnitd{br34dcrumbs_l34d_th3_w4y}

## Decoy flags (reject these if submitted)
foobarnitd{th4ts_th3_0ld_tr1ck}
   -> hidden in the biggest file, written backwards. This is on purpose: it catches
      anyone who found the old "SubDirectoTree" writeup online and used its trick.
Also three non-flag strings hidden in shorter deep paths:
   not_the_flag_keep_walking / wrong_turn_go_deeper / you_are_getting_warmer_maybe

## Optional hints (release later)
1. "The folders are more talkative than the files."
2. "Some paths are much longer than others."
3. "Each folder name is exactly one byte."

## Files in this challenge
- trailhead.zip    -> player file (1607 folders, 19 files)
- writeup_challenge3.txt -> full solution (organisers only)
