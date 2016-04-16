# Facebook Messenger Echo Bot
Facebook Launched Messenger API in F8 Conference. This opens up gate for many who want to build bots for Facebook Messenger.

This is a simple echo bot built using the APIs.

Setup
---------------------------
- Setup a Nodejs client running on HTTPS. Refer to awesome Digital Ocean resource for same [here]('https://www.digitalocean.com/community/tutorials/how-to-set-up-a-node-js-application-for-production-on-ubuntu-14-04')
- Facebook does not play nice with self signed certificates. Buy one from a provider else you can generate one for free from LetsEncrypt. Refer to [this](https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-14-04) guide for same.
- Follow steps mentioned at [Facebook Messenger API docs](https://developers.facebook.com/docs/messenger-platform/implementation) to create an app and a page required.
- Generate page access token
- Use token generated in previous step to make a cURL call and subscribe app to page.
- Fill relevant details in `conf.js` file.
- Start node server and complete the Webhook setup process.
- You are ready to go, bot should respond back with exact string sent.