# Octauthent Demo

Hi there 👋

Welcome the the Octauthent demo!

This simple website is composed of 2 pages:

- A [home page](https://demo.octauthent.com), accessible to everyone 🔓
- A [private page](https://demo.octauthent.com/private), protected by Octauthent 🔒

## Credentials

If you want to access the [private page](https://demo.octauthent.com/private), you'll need the following credentials:

**username**: `demo`

**password**: `octauthent`

## How it works

This website is **nothing more than 2 HTML files** hosted on GitHub Pages!

There is absolutely no code related to authentication, so everybody could (normally) access the private page

However, thanks to [Octauthent](https://octauthent.com), here is what happens when you access `demo.octauthent.com/private` from your browser:

1.  A DNS server recognizes the domain and responds with **a Cloudflare IP**
2.  Your browser **asks for the page** to the Cloudflare IP it received
3.  Cloudflare **runs the Octauthent code** to know what to do
4.  If Octauthent decides that **you are not allowed**, Cloudflare **responds with a customized login form**
5.  If Octauthent decides that **the page can be seen**:
    1.  Cloudflare **asks to Github Pages** the content of `demo.octauthent.com/private`
    2.  Github recognizes the address and **responds with the page content**
    3.  Cloudflare **sends the response** back to your browser
