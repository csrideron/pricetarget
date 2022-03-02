This project was interesting becasue it required both writing functional code, and ensuring that the widget performed a task accurately.

Coinbase Pro charges a small (depending on who you ask) fee per trade, both at both at entry and exit. 
That means that every trade starts at a loss. As such, I like to know what price I need to break even. I also like to get a sense of what the prise will be after certain percent increases, to temper expectations.

These are by no means complex calculations, but I got tired of doing them for every trade. So I wrote some code that, when given the price of the coin, outputs the following: 

1. Floor: My general trading strategy is to start with a stop-loss below the entry price. Then, I raise the limit as the price increases. Once the price decreases a certain amount, the position is closed. I usually start at 95% of the entry price, that way my loss isn't substantial if the price drops.
2. Breakeven price: This is the entry price multiplied by the percent increase needed to recover the principal.
3. 5%:  Breakeven price * 1.05%.
4. 10%:  Breakeven price * 1.10%. 

Determining the multiplication factor for the breakeven price took me longer to figure out than I'd like to admit. 
Again - this project was interesting because I had to ensure a precise output, in addition to ensuring functional code.

Overall, nothing very fancy here, but it has saved quite a bit of time with trading. 
My hope, as with any project, is to get this down to as few lines of code as possible. I'm obsesseively minimalist. Long-term, it'd also be nice to turn this into an API that automates my trading, given how algorithmic my process is.
