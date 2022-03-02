This was an interesting project in that in addition to writing functioning code, I had to make sure the code was mathematically precise. I wasn't just creating a webpage. i was creating a webpage that had to perform a specific task. It gave me an extra set of varialbes (no pun intended) to consider.

Coinbase Pro charges a small (depending on who you ask) fee per trade. In my case, it's 0.6 percent, both at entry and exit. 
What this means is that the moment I enter a trade, I'm at a loss. 

For every trade, I like to know a few things:
1. What price does the coin need to reach for me to break even? THe percent increase would have to compensate both for both fees. 
2. What would an increase of X% look like for this coin?

These are by no means complex calculations, but having to do them for every single trade I make got old. So I wrote some javascript that, when given the value of the coin, will tell me the following: 

1. Floor: My general trading strategy is to set a floor below the coin price, and then raise that floor as the price rises. If the price drops, the asset sells and i take a small loss, but I'm shielded from larger losses. The first floor is approximately at 95% of the entry price.
2. Breakeven price: This is the spotprice multiplied by the percent increase you'd need in the asset to get all of your principal back if you sold.
3. 5%:  Breakeven price * 1.05%.
4. 10%:  Breakeven price * 1.10%. 

Determining the multiplication factor for the breakeven price took me longer to figure out than I'd like to admit. 

Overall, nothing very fancy here, but it has saved quite a bit of time with trading.
