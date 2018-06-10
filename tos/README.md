## Think of Swim

### Strategy template

```
input tradeSize = 2;
def signal = <add buy condtion>;
addOrder(OrderType.BUY_TO_OPEN, signal, open[-1], tradeSize, Color.CYAN, Color.CYAN, "BUY");

def exit = <add sell condtion>;
addOrder(OrderType.SELL_TO_CLOSE, exit, open[-1], tradeSize, Color.RED, Color.RED,"SELL");

```

### Study Template

```
declare lower;
plot signal= RSI()."RSI" crosses above 34;
plot exit = <>;
```

### Painting

```
signal.SetPaintingStrategy(PaintingStrategy.LINE);

ARROW_DOWN, ARROW_UP, BOOLEAN_ARROW_DOWN, BOOLEAN_ARROW_UP, BOOLEAN_POINTS,
DASHES, HISTOGRAM, HORIZONTAL, LINE, LINE_VS_POINTS, LINE_VS_SQUARES, LINE_VS_TRIANGLES, POINTS,
SQUARED_HISTOGRAM, SQUARES, TRIANGLES, VALUES_ABOVE, VALUES_BELOW

```

See https://github.com/jshingler/TOS-and-Thinkscript-Snippet-Collection/blob/master/snippets.md
