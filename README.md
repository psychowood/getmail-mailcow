# getmail for mailcow

Python script that uses [IMAPClient](https://imapclient.readthedocs.io/) keep IMAP accounts synchronized, uses Local Mail Transfer Protocol.

Keeps your mailboxes synchronized in realtime instead of having to rely on a scheduled task the way mailcow does out of the box using IMAPsync.

This is mostly identical from Getmail: https://github.com/mailcow/mailcow-dockerized/issues/1554 I just added some specs to make it easier to deploy together with mailcow.

Current Known limitations:
- [ ] Can't sync to a remote server (must be run locally)
- [ ] Needs ssl with valid (not self signed) certificate
- [ ] Crashes when trying to sync very large folders
