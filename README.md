# defender-dump

Dump quarantined files from Windows Defender

## Description

Given the quarantined file in the current working directory, decrypt the file(s).

**Update:** for a more robust version supporting multiple AVs see [maldump](https://github.com/NUKIB/maldump)

## Usage

defender-dump.py --dump

###
Sample Files are both Eicar test files, one has the corresponding entries file, meaning file metadata can be recovered. The second does not, meaning the file can be decrypted but the original file name is not recovered.

- Place ResourceData file(s) in the same folder as Python script
- Place Entries folder file(s) in the directory also (optional)
- defender-dump.py --dump

## Limitation

The script will list and export only entries of the type "FILE". Any other types (like Registry) are not yet supported.

## License
[MIT](https://choosealicense.com/licenses/mit/)
