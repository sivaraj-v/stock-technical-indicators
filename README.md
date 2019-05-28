# ⛳️ Stock-Technical-Indicator 

## 🚦 Calculate Average True Range (ATR)
#####  ATR Sample Data
https://gist.github.com/zural/2e181ab0cbb3525d121ce4a4c6a28aa8

RunKit: https://runkit.com/zural/stock-indicator-study-atr

```
const SampleData = require('SampleData);
const { Indicator } = require('../../study/index');

const { ATR } = require('../../study/ATR');
const newStudyATR = new Indicator(new ATR());
console.log(newStudyATR.calculate(ATR_DATA));

Output
 [ ...
 	TrueRange: 26.75, 
 	SumTrueRange: 125.5999999999998,
	Value: 19.44443831563074
]

```
-------

## 🔃 Calculate Supertrend
Up trend is indicated as **Direction: 1**
Downtrend is indicated as **Direction: -1**
#####  Supertrend Sample Data
https://gist.github.com/zural/2e181ab0cbb3525d121ce4a4c6a28aa8

RunKit: https://runkit.com/zural/stock-indicator-study-supertrend

```
const SampleData = require('SampleData);
const { Indicator } = require('../../study/index');

const { Supertrend } = require('../../study/Supertrend');
const newStudySuperTrend = new Indicator(new Supertrend());
const calculateSupertrend = newStudySuperTrend.calculate(ATR_DATA, { period: 7, multiplier: 3 });
console.log(calculateSupertrend);

Output:
[
	Direction: 1,
	Up: 651.0916850531078,
	Down: 706.9636508963451,
	ActiveTrend: 651.0916850531078
]
```

**Social Connect**
https://www.linkedin.com/in/shivawebdeveloper/

**Contribute**
https://github.com/zural/stock-technical-indicators
