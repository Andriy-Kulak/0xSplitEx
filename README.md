## 0xSplit Example

- This is a basic example with rainbow kit, wagmi, 0xSplits
- it works for creating split with Polygon Mumbai.

Using:

- [0xSplits](https://www.0xsplits.xyz/)
- [RainbowKit](https://rainbowkit.com)
  - use this to log in with your wallet and test the app
- [wagmi](https://wagmi.sh) for hooks
- [Next.js](https://nextjs.org/)
- bootstrapped with [`create-rainbowkit`](https://github.com/rainbow-me/rainbowkit/tree/main/packages/create-rainbowkit)
- added basic prettier configs
- chakra ui for component library

## Getting Started

First, run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You should be able to log in on mumbai polygon test net. If you don't have it, please add mumbai test net using [chainlist](https://chainlist.org/)

In `pages/index.tsx` adjust the configs of recepients and controller before clicking "Create Split"

```ts
// ...
const args = {
  recipients: [
    {
      address: 'recepient add. 1',
      percentAllocation: 50.0,
    },
    {
      address: 'recepient add. 2',
      percentAllocation: 50.0,
    },
  ],
  distributorFeePercent: 1.0,
  controller: 'controller address',
}
```

## Adjusting Configs
