sub
===
Allows you to send out mass text messages to a list of subscribers.

### Installation

1) Download zip of the repository.
2) Run `composer install`
3) Create a database
4) Run `database.sql` on the database.
5) Add the connection info for the database in `config.php`.
6) Set up a twilio account.
7) Add the twilio info in `config.php`.
8) Upload everything to a server for hosting.
9) Provision a new phone number.
10) Point the webhook to your https://your-web-server/subscribe.php.  HTTP POST should be the method used.
11) `$subscribe_keyword` and `$unsubscribe_keyword` are the trigger words for your subscribers to be added and removed.
12) Once your admin (or broadcaster, the person who is sending out the notifications) has been enrolled in the database, you can set the `is_admin` field to `1`.

### Admin Usage
An admin can send an SMS with `broadcast` and then some message.  That message will be sent to all subscribers.

Lots of room for improvement.
