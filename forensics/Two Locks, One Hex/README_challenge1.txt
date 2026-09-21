# Two Locks, One Hex Editor

## Category
Forensics

## Difficulty
Easy-Medium

## Description  (what players see)
Our club's document scanner crashed halfway through writing a case file.
IT managed to pull one archive off the disk, but nothing will open it.
`unzip` refuses, and the one useful-looking file inside has no idea what it is.

Recover whatever the scanner was trying to save.

"the file isn't broken, it just forgot who it is." - GLUG sysadmin

## Topics
- Hex editing and file signatures (magic bytes)
- ZIP structure (local header vs End Of Central Directory record)
- PNG structure (8-byte signature + IHDR chunk)

## Hosting information
Attach chall.zip to the challenge for players to download.
Do NOT attach the writeup.

## Flag
foobarnitd{m4g1c_byt3s_n3v3r_l13_glug}

## Decoy flag (reject this if submitted)
foobarnitd{n0t_th3_r34l_0n3}

## Optional hint (release later)
"Zip files are read from the back. PNGs are recognised from the front."

## Files in this challenge
- chall.zip        -> player file (broken zip: missing 50 4B 05 06 at the end)
                      contains case/notes.txt (decoy) and case/scan.dat (PNG with wiped magic bytes)
- forensics_challenge_writeup.txt -> full solution (organisers only)
