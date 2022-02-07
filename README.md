# investor-days-fall21

Fall 2021 Quant SC Project by Leyla Winston, Morgan Lu, Syrah Vaswani, and Rohan Sanjay (Project Manager). We investigated heightened variability in option price movements on investor days. Check out our presentation [here](https://docs.google.com/presentation/d/1OMdCbCVdm1Ctyj82If7naslAkP7ya40nhJJYIRRVjVI/edit#slide=id.g102d6bd0591_0_0)!

Findings:

- Volume: spikes in volume mirror price fluctuations on investor days
- Moneyness: ATM and OTM options appear more volatile than ITM options on investor days
- Direction: put prices tend to move more the day before an investor day

Final presentation panelist feedback:

- Comparing investor days to earning calls could make a great academic paper
- Try to see if a pattern exists in when investor days happen along with whether there is usually specific fundamental information that drives price movements
- Consider overall market movement
- Look at IV and track deltas
- Note that strict risk management at trading firms generally won't allow for such large directional positions

## Project Timeline

### 11/29

Outline for presentation:

1. Title Slide - Rohan

2. Team intro (need a headshot from everyone) - Rohan 

3. Investor Day background - Rohan 

4. 1. What is an investor day
   2. What trends do we see on investor days (include a graph)
   3. Our hypothesis and project goals

5. Analysis slides

6. 1. Everyone can present a slide on their analysis

7. What we learned (finance, tools, etc.) - Leyla

8. Challenges - Morgan

9. Next steps - Syrah

### 11/22

Summary:

- Generated options chain returns by contract using groupby
  - Decided against implied volatility calculations because of issues with QuantConnect importing unsupported packages
- Brainstormed analysis steps and formulated the following plan to wrap up the project/semester
  - Work on analysis during meeting tomorrow and through this week
  - Discuss findings at next Monday's team meeting (11/29 4 PM DML East Asian-110B) and create presentation
  - Rehearse presentation Monday night ~30 mins (tentatively at 8:30 PM)
  - Present Tuesday during general meeting
  - Done team celebration lfggg

To do (**by 11/29**):

- Analysis work (refer to updated skeleton code [here](https://github.com/quantsc/investor-days-fall21/blob/main/rohans_code/research.ipynb))
  - Step 1: find an investor day for some company (change ticker and start/end date in getOptionDf function call)
  - Step 2: plots graphs for a column for every single contract (plotAllStrikesAndTypes function call)
    - Interesting columns: 'returns', 'close', 'volume'
  - Step 3: look for something interesting! Take screenshots of what you see and document
  - Guiding questions:
    - Do different parts of the options chain (moneyless - ATM, ITM, OTM) have different trends on investor days? Does one subset move more than others?
    - Do trends for calls and put with the same strike/expiry move in the directions we expect?
    - Are big volume changes correlated with big corresponding changes in price/returns?
- Presentation
  - We'll create an outline during tomorrow's general meeting and talk slides etc. 

### 11/15

Summary:

- First commits LFG (we'll never forget this day)
- Talked about calculating implied volatility for each option using Black Scholes with py_vollib package

### 11/9 - General Meeting

Summary:

- Learned command line basics and cloned GitHub repository
- Read through options basics tutorial on QuantConnect

To do (**by 11/15**)

- Watch this command line basics [video](https://www.youtube.com/watch?v=aKRYQsKR46I)
- Read these QuantConnect options tutorials
  - [General Features of Options](https://www.quantconnect.com/tutorials/introduction-to-options/general-features-of-options)
  - [Put-Call Parity and Arbitrage Strategies](https://www.quantconnect.com/tutorials/introduction-to-options/put-call-parity-and-arbitrage-strategies)
  - [Options Pricing](https://www.quantconnect.com/tutorials/introduction-to-options/options-pricing-black-scholes-merton-model)
  - [Historical Volatility and Implied Volatility](https://www.quantconnect.com/tutorials/introduction-to-options/historical-volatility-and-implied-volatility)

### 11/8 - Team Meeting

Summary: 

- Reviewed starter code
- Discussed options basics

### 11/1 - Team Meeting

Summary:

- Made team project check in [presentation](https://docs.google.com/presentation/d/1jru1xy_MMRq6dFX2kD2tH5IspbeE0qObgqWaQOGPWzE/edit)

To do ( **by 11/8**):

- Review options data analysis [starter code](https://github.com/quantsc/investor-days-fall21/blob/main/rohans_code/research.ipynb) and try making plots for other investor days
- Options reading
  - https://www.investopedia.com/options-basics-tutorial-4583012
  - https://optionalpha.com/options/basics
  - https://www.optionsplaybook.com/options-introduction/what-is-volatility/

### 10/25 - Team Meeting

Summary: 

- Pulled and graphed close prices of stocks in the research environment (different dates, frequences, etc.)
- Started looking into options and plotting prices at different strikes 

To do (**by 10/26**):

- Think about specific direction of project interest

### 10/19 - General Meeting

Summary: 

- Set weekly meeting time (Mondays 4 - 5)
- QuantConnect research notebook demo (pulling stock data)

To do (**by 10/26**):

- Read through research notebook documentation [here](https://www.quantconnect.com/docs/research/overview)
- Read through how to pull historical data [here](https://www.quantconnect.com/docs/research/historical-data)
- QuantConnect exercise
  - Create a new QuantConnect Algorithm in your account called "Investor Days"
  - Open the research.ipynb notebook in the left side bar
  - Pick a stock, pull it's historical price data over the past year, and plot it's close price
- Optional readings
  - [Python basics](https://www.freecodecamp.org/news/python-crash-course/)
  - [Pandas basics](https://pandas.pydata.org/pandas-docs/version/1.3/user_guide/10min.html)

### 10/5 - General Meeting

Summary:

- Team intros 
- Project direction interest
- Development workflow

To do (**by 10/12**):

- Create a QuantConnect [account](https://www.quantconnect.com/login)
- Complete Lesson 1 (Buy and Hold / Equities) of this [tutorial course](https://www.quantconnect.com/learning/course/1/boot-camp-101-us-equities)
- Fill out your availability for our weekly team meetings [here](https://lettucemeet.com/l/Dl2l8)
  - *note: we will meet the week of 10/17 and use that as a recurring meeting time slot so please fill out your availability accordingly*
- Feel free read up on investor days / project topics generally and add any interesting findings to our shared drive [here](https://drive.google.com/drive/u/0/folders/0AEPlvIHyEklGUk9PVA)



