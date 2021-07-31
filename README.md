# NextSimUpdate.io
👋 Hello, this is a simple site which tells people when the next update for Microsoft Flight Simulator is, it will show a countdown to each update, as-well as displaying the time and date of the release in the users timezone. Its primarily Javascript and HTML based and uses Jekyll to compile. https://jekyllrb.com/

At the moment the site is automatically built using Vercel. https://vercel.app/ However this may change if Bandwidth gets too high, I may opt to use Amazon AWS then. 
 
 ![image](https://user-images.githubusercontent.com/88237957/127741600-2a462250-d089-4cf6-8495-f402cd371b4c.png)

 
## How to build this repo

**Requirements**
- Ruby version 2.5.0 or higher, including all development headers (check your Ruby version using ruby -v)
- RubyGems (check your Gems version using gem -v)
- GCC and Make (check versions using gcc -v,g++ -v, and make -v)

Please follow https://jekyllrb.com/docs/installation/

1. Clone this REPO
2. Run `Jekyll serve`

## How to contribute
I've tried to make contributions as easy as possible, hence why I'm using Jekyll!
(You don't need any programming experience to be able to contribute, just a basic understanding of Git)

Take a look at https://github.com/theyetty/nextsimupdate/tree/main/_release_dates

This contains MD (Markdown) files of every update coming to Microsoft Flight Simulator.

To add a new update just make a pull request with a .md file, the format is as follows

```
---
title: PATCH - 1.14.6.0
type: patch
to_date: "26 March 2021 15:00:00 UTC"
layout: countdown
background_image: "https://cdn.cloudflare.steamstatic.com/steam/apps/1250410/ss_a2a3aa69d655252087ace6eac887382f1e0582fa.1920x1080.jpg?t=1623947484"
background_color: "000"
---
```

Also please edit: https://github.com/theyetty/nextsimupdate/blob/main/_config.yml

Look for order: and add the md file in the right order 
(I cant get Jekylls auto ordering to work right atm, so this is manual for now)

- title: is what its called, should start with PATCH, WORLD UPDATE OR SIM UPDATE
- type: patch, worldupdate, simupdate
- to_date: Must follow this pattern e.g. 01 January 2022 10:00:00 UUTC
- layout: countdown (its always this for now)
- background_image: the background image, (make sure its MSFS related so its covered under the fair use policy Microsoft grant)
- background_color: if no image, a color in HEX

If you don't want to do this, you can open an **Issue** at the top and let me know about a change, and I can make it! :)

If you wanna make more complex changes, go ahead and I will review the Pull Requests :)
