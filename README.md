## Getting Started

The obvious stuff

```shell
yarn
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser and enjoy.

## The stack

Nextjs + Redux-toolkit + tailwind + scss

## Info

- Was written in a tight timeframe(less than 3 workdays) so a quite a few corners were cut with a garage / hackathon mindset. Willing to answer any question regarding design / code structure.
- Nextjs + tailwind + scss I think is a no-brainer(maybe Windi but haven't tried it yet)
- Tried Redux, MobX, React Context, Recoil, Redux toolkit. Found Redux toolkit to be the most Developer Friendly with no known performance issues so used that.
- Focused on getting quick results ASAP using tailwind to it's fullest. As a result some components are probably possible to extract but did not for time's sake
- In hindsight using SWR would have been more efficient but the app was ISR at the beginning and didn't think refactoring would be worth the time after switching to CSR.
- Definitely not as polished as I would be comfortable with atm, but the structure is similar to what I would do for this type of project and should give you a general idea of how I work.
- Commit naming is terrible, but who does proper conventional commits in the beginning of a project? Personally think it's a waste of time in the early stages of a project
- Used https://cosmos.directory/ api for ease of development
- Switched Uptimes to participated blocks as it's something I would probably have suggested to a designer if we were working together
- Added the validator's image to the page

## Known issues

- API is terribly unstable. You're [not going to get transaction data consistently](https://www.loom.com/share/23d4305f4bf84e9d9154f41a880065e6)
- Does say relayers, but it's validators atm. I couldn't find easily accessible relayer public data
- Heartbeat was set to uptime, Broadcaster was set to max(uptime - 0~2, 0)
- ReactTooltip doesn't work on first hover & tooltips don't disappear on DEV(known issue)
- No SEO
- tx table is not very responsive. Benchmarking Mintscan's method of displaying txs in mobile would be a nice way to go

## Deploying

Use Vercel or netlify. Shouldn't need any more than that
