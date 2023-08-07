# pinescript
collection of my scripts

## 3rd party strategies:
- https://github.com/vikaschouhan/algotrade/tree/master/pinescript
- https://github.com/aceri/tradingview_pinescript
- https://github.com/oguzhandilber/PineScripts
- https://github.com/pradip-interra/PineScripts/tree/main
- https://github.com/Alorse/pinescript-strategies

## 3rd party studies:
- https://github.com/harryguiacorn/tradingview/blob/main/CandlestickInsideBar.pine


### Strategies
It is important to add these line of code to every strategy:
```py
// LIVEMODE:: ENABLE / DISABLE
enableLiveTest = input.bool(false, title="Enable live mode and stop backtesting", group="Livemode / Backtesting")
curDate = timestamp('2023, 08, 06')
targetDate = input.time(curDate, title="Start live mode from:", group="Livemode / Backtesting")
// LIVEMODE:: END

if enableLiveTest == false or time > targetDate

```