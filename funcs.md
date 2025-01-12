# All Supported Indicators and Functions 所有支持的指标和函数

* [Overlap Studies](func_groups/overlap_studies.md)
* [Momentum Indicators](func_groups/momentum_indicators.md)
* [Volume Indicators](func_groups/volume_indicators.md)
* [Volatility Indicators](func_groups/volatility_indicators.md)
* [Price Transform](func_groups/price_transform.md)
* [Cycle Indicators](func_groups/cycle_indicators.md)
* [Pattern Recognition](func_groups/pattern_recognition.md)
* [Statistic Functions](func_groups/statistic_functions.md)
* [Math Transform](func_groups/math_transform.md)
* [Math Operators](func_groups/math_operators.md)

#### [Overlap Studies](func_groups/overlap_studies.md)  重叠研究

```
BBANDS               Bollinger Bands
DEMA                 Double Exponential Moving Average
EMA                  Exponential Moving Average
HT_TRENDLINE         Hilbert Transform - Instantaneous Trendline
KAMA                 Kaufman Adaptive Moving Average
MA                   Moving average
MAMA                 MESA Adaptive Moving Average
MAVP                 Moving average with variable period
MIDPOINT             MidPoint over period
MIDPRICE             Midpoint Price over period
SAR                  Parabolic SAR
SAREXT               Parabolic SAR - Extended
SMA                  Simple Moving Average
T3                   Triple Exponential Moving Average (T3)
TEMA                 Triple Exponential Moving Average
TRIMA                Triangular Moving Average
WMA                  Weighted Moving Average
```

#### [Momentum Indicators](func_groups/momentum_indicators.md)  动量指标

```
ADX                  Average Directional Movement Index
                    平均趋向指数 ？
ADXR                 Average Directional Movement Index Rating

APO                  Absolute Price Oscillator  绝对价格振荡器
AROON                Aroon
AROONOSC             Aroon Oscillator

BOP                  Balance Of Power           力量平衡
                    [ BOP = \frac{(Close - Open)}{(High - Low)} ]
CCI                  Commodity Channel Index    商品通道指数
                    [ CCI = \frac{TP - SMA(TP, n)}{\frac{0.015 \times MAD(TP, n)}} ]
CMO                  Chande Momentum Oscillator 钱德动量摆动指标
                    [ CMO = \frac{(Su - Sd)}{(Su + Sd)} \times 100 ]
DX                   Directional Movement Index 方向性移动指数
MACD                 Moving Average Convergence/Divergence
MACDEXT              MACD with controllable MA type
MACDFIX              Moving Average Convergence/Divergence Fix 12/26
MFI                  Money Flow Index       一段时间内，资金流入流出的比例
MINUS_DI             Minus Directional Indicator
MINUS_DM             Minus Directional Movement
MOM                  Momentum
PLUS_DI              Plus Directional Indicator
PLUS_DM              Plus Directional Movement
PPO                  Percentage Price Oscillator
ROC                  Rate of change : ((price/prevPrice)-1)*100
ROCP                 Rate of change Percentage: (price-prevPrice)/prevPrice
ROCR                 Rate of change ratio: (price/prevPrice)
ROCR100              Rate of change ratio 100 scale: (price/prevPrice)*100
RSI                  Relative Strength Index
STOCH                Stochastic
STOCHF               Stochastic Fast
STOCHRSI             Stochastic Relative Strength Index
TRIX                 1-day Rate-Of-Change (ROC) of a Triple Smooth EMA
ULTOSC               Ultimate Oscillator
WILLR                Williams' %R
```

#### [Volume Indicators](func_groups/volume_indicators.md)  成交量指标

```
AD                   Chaikin A/D Line               ？会加昨日 A/D 吗
                    ((close - low) - (high - close)) / (high - low) * volume
ADOSC                Chaikin A/D Oscillator
                    EMA(AD Line, short_period) - EMA(AD Line, long_period)
OBV                  On Balance Volume              成交量正负叠加
```

#### [Cycle Indicators](func_groups/cycle_indicators.md)    波动性指标

```
HT_DCPERIOD          Hilbert Transform - Dominant Cycle Period
HT_DCPHASE           Hilbert Transform - Dominant Cycle Phase
HT_PHASOR            Hilbert Transform - Phasor Components
HT_SINE              Hilbert Transform - SineWave
HT_TRENDMODE         Hilbert Transform - Trend vs Cycle Mode
```

#### [Price Transform](func_groups/price_transform.md)  价格指标

```
AVGPRICE             Average Price
                    [ \text{AVGPRICE} = \frac{\text{High} + \text{Low} + \text{Open} + \text{Close}}{4} ]
                    单个交易日的平均价格
MEDPRICE             Median Price
                    [ \text{MEDPRICE} = \frac{\text{High} + \text{Low}}{2} ]
                    单个交易日的中点价格
TYPPRICE             Typical Price
                    [ \text{TYPPRICE} = \frac{\text{High} + \text{Low} + 2 \times \text{Close}}{4} ]
                    用于计算单个交易日的典型价格
WCLPRICE             Weighted Close Price
                    [ \text{WCLPRICE} = \frac{\text{High} + \text{Low} + 2 \times \text{Close}}{4} ]
                    用于计算单个交易日的加权收盘价
```

#### [Volatility Indicators](func_groups/volatility_indicators.md)  周期指标

```
ATR                  Average True Range
                    [ \text{TR} = \max(\text{High} - \text{Low}, |\text{High} - \text{Previous Close}|, |\text{Low} - \text{Previous Close}|) ]
                    简单移动平均、指数移动平均
                    可以作为止损点，止盈点，例如，设置止损点为当前价格减去 ATR 的 2 倍
NATR                 Normalized Average True Range
                    NATR 是 ATR 除以收盘价并乘以 100，以百分比形式表示
TRANGE               True Range
                    TRANGE 是计算 ATR（Average True Range）的基础，用于衡量单个交易日内的价格波动范围
```

#### [Pattern Recognition](func_groups/pattern_recognition.md)  形态识别

```
CDL2CROWS            Two Crows
CDL3BLACKCROWS       Three Black Crows
CDL3INSIDE           Three Inside Up/Down
CDL3LINESTRIKE       Three-Line Strike
CDL3OUTSIDE          Three Outside Up/Down
CDL3STARSINSOUTH     Three Stars In The South
CDL3WHITESOLDIERS    Three Advancing White Soldiers
CDLABANDONEDBABY     Abandoned Baby
CDLADVANCEBLOCK      Advance Block
CDLBELTHOLD          Belt-hold
CDLBREAKAWAY         Breakaway
CDLCLOSINGMARUBOZU   Closing Marubozu
CDLCONCEALBABYSWALL  Concealing Baby Swallow
CDLCOUNTERATTACK     Counterattack
CDLDARKCLOUDCOVER    Dark Cloud Cover
CDLDOJI              Doji
CDLDOJISTAR          Doji Star
CDLDRAGONFLYDOJI     Dragonfly Doji
CDLENGULFING         Engulfing Pattern
CDLEVENINGDOJISTAR   Evening Doji Star
CDLEVENINGSTAR       Evening Star
CDLGAPSIDESIDEWHITE  Up/Down-gap side-by-side white lines
CDLGRAVESTONEDOJI    Gravestone Doji
CDLHAMMER            Hammer
CDLHANGINGMAN        Hanging Man
CDLHARAMI            Harami Pattern
CDLHARAMICROSS       Harami Cross Pattern
CDLHIGHWAVE          High-Wave Candle
CDLHIKKAKE           Hikkake Pattern
CDLHIKKAKEMOD        Modified Hikkake Pattern
CDLHOMINGPIGEON      Homing Pigeon
CDLIDENTICAL3CROWS   Identical Three Crows
CDLINNECK            In-Neck Pattern
CDLINVERTEDHAMMER    Inverted Hammer
CDLKICKING           Kicking
CDLKICKINGBYLENGTH   Kicking - bull/bear determined by the longer marubozu
CDLLADDERBOTTOM      Ladder Bottom
CDLLONGLEGGEDDOJI    Long Legged Doji
CDLLONGLINE          Long Line Candle
CDLMARUBOZU          Marubozu
CDLMATCHINGLOW       Matching Low
CDLMATHOLD           Mat Hold
CDLMORNINGDOJISTAR   Morning Doji Star
CDLMORNINGSTAR       Morning Star
CDLONNECK            On-Neck Pattern
CDLPIERCING          Piercing Pattern
CDLRICKSHAWMAN       Rickshaw Man
CDLRISEFALL3METHODS  Rising/Falling Three Methods
CDLSEPARATINGLINES   Separating Lines
CDLSHOOTINGSTAR      Shooting Star
CDLSHORTLINE         Short Line Candle
CDLSPINNINGTOP       Spinning Top
CDLSTALLEDPATTERN    Stalled Pattern
CDLSTICKSANDWICH     Stick Sandwich
CDLTAKURI            Takuri (Dragonfly Doji with very long lower shadow)
CDLTASUKIGAP         Tasuki Gap
CDLTHRUSTING         Thrusting Pattern
CDLTRISTAR           Tristar Pattern
CDLUNIQUE3RIVER      Unique 3 River
CDLUPSIDEGAP2CROWS   Upside Gap Two Crows
CDLXSIDEGAP3METHODS  Upside/Downside Gap Three Methods
```

#### [Statistic Functions](func_groups/statistic_functions.md)  统计函数

```
BETA                 Beta
CORREL               Pearson's Correlation Coefficient (r)
LINEARREG            Linear Regression
LINEARREG_ANGLE      Linear Regression Angle
LINEARREG_INTERCEPT  Linear Regression Intercept
LINEARREG_SLOPE      Linear Regression Slope
STDDEV               Standard Deviation
TSF                  Time Series Forecast
VAR                  Variance
```

#### [Math Transform](func_groups/math_transform.md)    数学变换

```
ACOS                 Vector Trigonometric ACos
ASIN                 Vector Trigonometric ASin
ATAN                 Vector Trigonometric ATan
CEIL                 Vector Ceil
COS                  Vector Trigonometric Cos
COSH                 Vector Trigonometric Cosh
EXP                  Vector Arithmetic Exp
FLOOR                Vector Floor
LN                   Vector Log Natural
LOG10                Vector Log10
SIN                  Vector Trigonometric Sin
SINH                 Vector Trigonometric Sinh
SQRT                 Vector Square Root
TAN                  Vector Trigonometric Tan
TANH                 Vector Trigonometric Tanh
```

#### [Math Operators](func_groups/math_operators.md)    数学运算符

```
ADD                  Vector Arithmetic Add
DIV                  Vector Arithmetic Div
MAX                  Highest value over a specified period
MAXINDEX             Index of highest value over a specified period
MIN                  Lowest value over a specified period
MININDEX             Index of lowest value over a specified period
MINMAX               Lowest and highest values over a specified period
MINMAXINDEX          Indexes of lowest and highest values over a specified period
MULT                 Vector Arithmetic Mult
SUB                  Vector Arithmetic Substraction
SUM                  Summation
```

[Documentation Index](doc_index.md)
