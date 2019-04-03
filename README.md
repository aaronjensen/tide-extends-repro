# Tide extends repro

Tide does not properly support extending configs via packages.

Install dependencies via `yarn`

To reproduce, visit `sub/index.ts` and make a change. You should see:


```
error in process filter: tsconfig file not found at
"/Users/aaronjensen/Source/temp/tide-extends-repro/sub/base/tsconfig.json".
```

Compare this to running `yarn tsc` in the `sub` directory, which does find the config.
