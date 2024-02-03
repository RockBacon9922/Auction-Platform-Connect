# Auction Platform Connect

This is a [Plasmo extension](https://docs.plasmo.com/) project bootstrapped with [`plasmo init`](https://www.npmjs.com/package/plasmo).

## Getting Started

```bash
pnpm i && pnpm dev
```

## About

Auction Platform Connect was my attempt to join auction platforms together so that only one auction clerk would be required to run an auction on multiple platforms.

Unfortunately, the platform Bidspirit beat me to the gun with this project and released their own version of this idea, making my project redundant.

The current status of this project is that it is nearly finished. State is managed with Redux and the UI is built with React. The backend content scripts integrate seamlessly with easylive auctions.

## How it works

The backend content scripts are injected into the auction platforms and listen for DOM events. All the events update the Redux store and the UI is updated from this. When the UI is updated it updates the Redux store and the content scripts listen for these changes and update the DOM accordingly. This approach is simple and allows for a seamless integration with the auction platforms with a single source of truth.

## Technologies

- Plasmo
- React
- Redux

## Moving on from this project

I am still proud of this project and the over 500 hours I have put into it. I have moved on and will continue to work on other software to improve the auction industry.

## License

This project is licensed under the GNU AFFERO GENERAL PUBLIC LICENSE. See the [LICENSE](LICENSE) file for details.
