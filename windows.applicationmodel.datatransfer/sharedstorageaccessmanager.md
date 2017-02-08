---
-api-type: winrt class
---
 The source app calls the [AddFile](sharedstorageaccessmanager_addfile.md) method to get the sharing token that it passes to the target app, which it launches with a Uri.
 The target app calls the [RedeemTokenForFileAsync](sharedstorageaccessmanager_redeemtokenforfileasync.md) method to get the shared file.
 Optionally, the source app can call the [RemoveFile](sharedstorageaccessmanager_removefile.md) method to revoke a token that it obtained previously by calling the [AddFile](sharedstorageaccessmanager_addfile.md) method.
 A sharing token can only be redeemed one time. After that, the token is no longer valid.
 A sharing token expires after 14 days and is no longer valid.
 The source app cannot get more than one thousand sharing tokens. After a token is redeemed, removed, or expires, however, it no longer counts against the quota of the source app.