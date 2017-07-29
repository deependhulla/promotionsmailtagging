# promotionsmailtagging

Theses Days we receive many Promotional mail , be in form of advertisement, newsletter, mailing list, some bulk marketing mails...etc. which irritated many specially in work mailbox. Google's Gmail has got a better algorithm to filter and put it under tab. but to have similar feature we need to keep on adding filter on our local email clients. to have server side filter with global tagging is now possible with spamassassin with dovecot sieve as filter on server side.

Copy promotionsmailtagging folder into /etc/spamassassin/ (on some system its /etc/mail/spamassassin/) 

Add the Lines of spamassassin/add_to_local.cf into /etc/mail/spamassassin/local.cf

Basic content catch has been added in [promotionsmailtagging/promotions.ini](spamassassin/promotionsmailtagging/promotions.ini) file you can add more if you want.

If you Mail system support Dovecot Sieve (Service side Filter) filter, you can use the sample given [dovecot_default.sieve](dovecot_default.sieve) to apply same.

In your ThirdParty Email Client like MS Outlook you can add a filter "X-Spam-Promotions" "YES" than move to Promotional Folder.

