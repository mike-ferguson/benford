
Determines if specific Data conform to Benford's Law.

Benford's Law states (from Wikipedia):

*Benford's Law, also called the Newcomb–Benford law, the law of anomalous numbers, or the first-digit law, is an observation about the frequency distribution of leading digits in many real-life sets of numerical data. The law states that in many naturally occurring collections of numbers, the leading digit is likely to be small.*

The fequencies of the digits are summarized by the equation *p(d) = log10((d+1)/d)*, where d are the digits 1-9.

The main purpose of this code is to tell whether or not a dataset has been corrupted or is fradualent, as it is suspicous if it does not obey the above law.

Wikipedia lists some restrictions on the data:

**Distributions that can be expected to obey Benford's law**
When the mean is greater than the median and the skew is positive
Numbers that result from mathematical combination of numbers: e.g. quantity × price
Transaction level data: e.g. disbursements, sales

**Distributions that would not be expected to obey Benford's law**
Where numbers are assigned sequentially: e.g. check numbers, invoice numbers
Where numbers are influenced by human thought: e.g. prices set by psychological thresholds ($1.99)
Accounts with a large number of firm-specific numbers: e.g. accounts set up to record $100 refunds
Accounts with a built-in minimum or maximum

The provided code looks at various Kaggle sales datasets that meet the above criteria. 
