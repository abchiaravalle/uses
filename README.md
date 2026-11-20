<p align="center">
  <a href="https://amplifi.studio">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="assets/amplifi-logo-dark-bg.svg">
      <img src="assets/amplifi-logo-light-bg.svg" alt="amplifi.studio" width="220">
    </picture>
  </a>
</p>

# uses

My favorite tools. Some are open source, some are paid. Each one has tags so you know which is which before you click.

**Tags:** `open source` code is public · `source available` code is public, but the license limits how you can use it · `self-host` you can run it on your own server · `free` costs nothing · `free tier` you can try it without paying · `paid` costs money

**Sections:** [Sales and CRM](#sales-and-crm) · [AI and notes](#ai-and-notes) · [Automation and documents](#automation-and-documents) · [Websites and analytics](#websites-and-analytics) · [Video and feeds](#video-and-feeds) · [Network, passwords and Mac](#network-passwords-and-mac) · [Stuff I built](#stuff-i-built)

## Sales and CRM

### [Twenty](https://twenty.com)

`open source` `self-host` `paid`

A CRM you can run on your own server for free, or use on their hosted cloud. You can add your own objects, fields, views and workflows without writing code, and there's an API and an apps framework for when you want more.

- Code: [twentyhq/twenty](https://github.com/twentyhq/twenty). Mostly AGPLv3, and a few enterprise files carry a separate commercial license.
- Cost: self-hosting is free. The hosted cloud starts at $9 per user per month, billed yearly.

### [MoltSets](https://moltsets.com)

`paid` `free tier`

B2B contact and company data through an API: work emails, mobile numbers, job titles and company info. There's no app to click around in. You pull the data into a spreadsheet, a CRM, a script or an AI tool. Each email goes through validation and comes back with a risk score.

- Docs: [developer.moltsets.com](https://developer.moltsets.com)
- Cost: the free tier gives you 1,000 calls with no card. Paid plans start at $27 a month for unlimited data under a fair use policy. Mobile numbers cost extra through a monthly add-on, about $0.15 each.

## AI and notes

### [Hermes Agent](https://github.com/NousResearch/hermes-agent)

`open source` `self-host` `free`

An AI agent from Nous Research that runs on my own machine. I talk to it from Discord, and it keeps memory between chats, runs scheduled jobs, and can use a browser, a terminal and the desktop. It also writes and updates its own how-to notes (it calls them skills) as it learns how I like things done.

- Code: [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent), MIT license.
- Cost: the agent is free. You pay for whichever AI model you connect to it.

### [Obsidian](https://obsidian.md)

`free` `paid`

A notes app that keeps everything as plain Markdown files in a folder on your computer. It sits next to Hermes because it's Hermes's long-term memory. The agent's always-on memory stays short, a list of pointers and standing rules. The full detail lives in my Obsidian vault: client notes, how each server is set up, my preferences, and a daily log of what got done. Hermes reads a note when a task needs it and writes back what it learned. I open the same vault in Obsidian to read, search and fix anything it wrote. The vault is a private git repo, so every change has history, and [qmd](https://github.com/tobi/qmd) (open source) lets the agent search it by meaning, not only exact words.

- Not open source, but the app is free, including for work. Sync is $4 a month and Publish is $8 a month, both billed yearly. You don't need either one to use a git repo the way I do.

### [LM Studio](https://lmstudio.ai)

`free`

Download and run AI models on your own Mac. You can chat with them in the app or serve them to other tools through a local API, so nothing leaves your machine.

- The app isn't open source. Its command-line tool ([lmstudio-ai/lms](https://github.com/lmstudio-ai/lms)) and SDKs are MIT.

### [Open WebUI](https://openwebui.com)

`source available` `self-host` `free`

A ChatGPT-style chat page you run yourself. It connects to local models (Ollama, LM Studio) or cloud ones (OpenAI, Anthropic, anything compatible), and handles document search, web search, voice and image tools. You can extend it with Python.

- Code: [open-webui/open-webui](https://github.com/open-webui/open-webui). It uses its own Open WebUI License, a BSD-style license with one extra rule: you can't remove or change the Open WebUI name and logo if more than 50 people use your copy in a 30-day period, unless you have their permission or an enterprise license.

## Automation and documents

### [n8n](https://n8n.io)

`source available` `self-host` `paid`

Drag-and-drop workflow automation, like Zapier, with hundreds of app connections, code steps when you need them, and AI steps.

- Code: [n8n-io/n8n](https://github.com/n8n-io/n8n). It uses n8n's Sustainable Use License, which isn't open source: you can self-host it free for your own business, but you can't resell it as a hosted service. Some enterprise features need a paid license. There's also a paid cloud version.

### [OpenSign](https://www.opensignlabs.com)

`open source` `self-host`

E-signatures, a free alternative to DocuSign. Upload a PDF, place the fields, send it out, and get back a signed copy with an audit trail.

- Code: [OpenSignLabs/OpenSign](https://github.com/OpenSignLabs/OpenSign), mostly AGPLv3.

### [Paperless-ngx](https://github.com/paperless-ngx/paperless-ngx)

`open source` `self-host` `free`

Scan or drop in a document and it reads the text, tags it, and makes it searchable.

- Code: [paperless-ngx/paperless-ngx](https://github.com/paperless-ngx/paperless-ngx), GPLv3.

## Websites and analytics

### [OpenSEO](https://openseo.so)

`open source` `self-host` `paid`

An open-source alternative to Semrush and Ahrefs: keyword research, rank tracking, competitor insights, backlinks, site audits and AI visibility. It comes with a connector for AI agents (MCP), so Hermes plugs into it and pulls SEO data on its own. I run my own copy on Cloudflare.

- Code: [every-app/open-seo](https://github.com/every-app/open-seo), MIT.
- Cost: there's no subscription when you self-host. You bring your own DataForSEO API key and pay only for the data you pull. My copy also needs Cloudflare's $5 a month Workers plan. The hosted version is $10 a month.

### [Rybbit](https://rybbit.com)

`open source` `self-host` `paid`

Website analytics without cookies, a privacy-friendly Google Analytics alternative. Pageviews, sources, funnels, goals, user journeys and web vitals, all on one dashboard.

- Code: [rybbit-io/rybbit](https://github.com/rybbit-io/rybbit), AGPLv3.
- Cost: self-hosting is free. The cloud starts at $13 a month (billed yearly) for 100k pageviews, after a 7-day free trial.

### [Shlink](https://shlink.io)

`open source` `self-host` `free`

Your own short links on your own domain, with click stats and QR codes.

- Code: [shlinkio/shlink](https://github.com/shlinkio/shlink), MIT.

### [Uptime Kuma](https://github.com/louislam/uptime-kuma)

`open source` `self-host` `free`

Checks your websites and servers every minute or so and pings you on Slack, Discord, email and dozens of other apps when one goes down. Comes with public status pages.

- Code: [louislam/uptime-kuma](https://github.com/louislam/uptime-kuma), MIT.

## Video and feeds

### [MeTube](https://github.com/alexta69/metube)

`open source` `self-host` `free`

A web page for downloading videos from YouTube and hundreds of other sites. Paste a link and it saves the file to your server. It runs on [yt-dlp](https://github.com/yt-dlp/yt-dlp).

- Code: [alexta69/metube](https://github.com/alexta69/metube), AGPLv3.

### [RSSHub](https://docs.rsshub.app)

`open source` `self-host` `free`

Makes RSS feeds for sites that don't offer one, so you can follow them in any feed reader.

- Code: [DIYgod/RSSHub](https://github.com/DIYgod/RSSHub), AGPLv3.

## Network, passwords and Mac

### [Tailscale](https://tailscale.com)

`free tier` `paid`

Puts all your computers, phones and servers on one private network, wherever they are. I use it to reach my home servers from anywhere without opening anything to the internet.

- The apps are open source ([tailscale/tailscale](https://github.com/tailscale/tailscale), BSD-3-Clause). The service that links your devices is Tailscale's own.
- Cost: the Personal plan is free for up to 6 users with unlimited devices.

### [Bitwarden](https://bitwarden.com)

`open source` `self-host` `free tier` `paid`

A password manager with end-to-end encryption, passkeys, and apps for every browser, phone and computer. The free plan covers unlimited passwords and devices.

- Code: [bitwarden/clients](https://github.com/bitwarden/clients) (GPLv3) and [bitwarden/server](https://github.com/bitwarden/server) (AGPLv3). A few business features use Bitwarden's own license.

### [Vaultwarden](https://github.com/dani-garcia/vaultwarden)

`open source` `self-host` `free`

A lightweight password server you host yourself that works with the regular Bitwarden apps and browser extensions. It covers nearly everything Bitwarden's own server does, including sharing, attachments, Send and two-factor login, and it's built to be lighter to self-host than Bitwarden's official server. I run my own copy. It's unofficial and not affiliated with Bitwarden.

- Code: [dani-garcia/vaultwarden](https://github.com/dani-garcia/vaultwarden), AGPLv3.

### [BlueBubbles](https://bluebubbles.app)

`open source` `self-host` `free`

iMessage on Android, Windows and Linux. You run the BlueBubbles server on a Mac that stays signed in to your Apple ID, and it forwards your iMessages to the BlueBubbles apps on your other devices.

- Code: [BlueBubblesApp/bluebubbles-server](https://github.com/BlueBubblesApp/bluebubbles-server), Apache-2.0. It needs macOS 10.15 or newer.

### [LocalSend](https://localsend.org)

`open source` `free`

AirDrop that works between any devices on the same Wi-Fi: Mac, Windows, Linux, iPhone and Android. Files go straight from one device to the other, no account needed.

- Code: [localsend/localsend](https://github.com/localsend/localsend), Apache-2.0.

### [Raycast](https://www.raycast.com)

`free tier` `paid`

A Mac launcher that replaces Spotlight: apps, clipboard history, snippets, window snapping, a calculator, and thousands of extensions.

- Not open source. The free plan covers the core features. Pro, which adds AI, starts at $10 a month.

## Stuff I built

### [loltools](https://github.com/abchiaravalle/loltools)

`open source` `free`

Small browser tools that do their work on your device, with no uploads: merge and compress PDFs, make QR codes, and convert iPhone HEIC photos to JPG or PNG.

### [findmyip.lol](https://findmyip.lol)

`open source` `free`

Shows your IP address. No trackers, no analytics, no cookies. The whole thing is one HTML file.

- Code: [abchiaravalle/findmyip.lol](https://github.com/abchiaravalle/findmyip.lol), MIT.

### [cad-studio-renders](https://github.com/abchiaravalle/cad-studio-renders)

`open source` `free`

Drop in a CAD file and get studio product shots, transparent cut-outs, and a 3D/AR viewer you can host yourself. It uses Blender and OpenCascade and runs on your own machine. It also ships as an AI agent skill.

- Code: MIT.

### [lwp, a LocalWP CLI](https://github.com/abchiaravalle/ac-amplifi-localwp-cli)

`open source` `free`

Start, stop and create [Local](https://localwp.com) WordPress sites, run WP-CLI against any of them, and open site shells from the terminal on a Mac. It's unofficial and not affiliated with WP Engine.

- Code: MIT.

---

From [amplifi.studio](https://amplifi.studio). Prices and licenses were checked in November 2026. They change, so check the link before you buy.
