# Volatility-Prediction
predict short-term volatility for hundreds of stocks across different sectors


Weighted averaged price

The order book is also one of the primary source for stock valuation. A fair book-based valuation must take two factors into account: the level and the size of orders. In this competition we used weighted averaged price, or WAP, to calculate the instantaneous stock valuation and calculate realized volatility as our target.

The formula of WAP can be written as below, which takes the top level price and volume information into account:

WAP=BidPrice1∗AskSize1+AskPrice1∗BidSize1BidSize1+AskSize1
 
As you can see, if two books have both bid and ask offers on the same price level respectively, the one with more offers in place will generate a lower stock valuation, as there are more intended seller in the book, and more seller implies a fact of more supply on the market resulting in a lower stock valuation.

Note that in most of cases, during the continuous trading hours, an order book should not have the scenario when bid order is higher than the offer, or ask, order. In another word, most likely, the bid and ask should never be in cross.
