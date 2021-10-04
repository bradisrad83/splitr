## Splitr

Splitr is a minimalist, dependency-free, *near 100% precise* splitting engine. This can be used for traffic plitting, or any other implimentation you need to split an outcome. **Sum of weights must equal 100.**

Example:

```
    const options: SplitOption[] = [
      {
        weight: 10,
        value: "10% of the time",
      },
      {
        weight: 20,
        value: "20% of the time",
      },
      {
        weight: 70,
        value: "70% of the time",
      },
    ];

    const splitr = new Splitr(options);

    let result = splitr.run();

    // "70% of the time" (most likely)
```
## Accuracy

Currently, the accuracy has been ~99.95% - 99.97%.

#### Notes:

- To test, run `npm test`
