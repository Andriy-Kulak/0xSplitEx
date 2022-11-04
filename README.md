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
- [chakra ui](https://chakra-ui.com/) for component library

## Getting Started

1. First, run the development server:

```bash
npm run dev
```

2. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

3. You should be able to log in with wallet on mumbai polygon test net. If you don't have it, please add mumbai test net using [chainlist](https://chainlist.org/)

4. In `pages/index.tsx` adjust the configs of recepients and controller

```ts
// ...
const args = {
  recipients: [
    {
      address: '...recepient add. 1',
      percentAllocation: 50.0,
    },
    {
      address: '...recepient add. 2',
      percentAllocation: 50.0,
    },
  ],
  distributorFeePercent: 1.0,
  controller: '...controller address',
}
```

5. Once updated, you can click "Create Split"
