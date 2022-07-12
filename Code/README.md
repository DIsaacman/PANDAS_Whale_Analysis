# How To Pull Asset Data With Google Sheets

Gather closing asset prices using *GOOGLE FINANCE* in google sheets and return Assets/Securities in Date Range

 ### How to Create Your Master Template
 
- Make a Copy [^1]
- Insert Dates and Ticker
- Export to .CSV 
- Use Python and PANDAS for Portfolio Analysis and Backtesting. 


### Syntax



`GOOGLEFINANCE(ticker, [attribute], [start_date], [end_date|num_days], [interval])` [^2]



### Examples



Gather Data for Stocks - AMD (Advanced Micro Devices) from 5/9/2019 until today's date.


```

=GOOGLEFINANCE("AMD","Price","5/9/2019",Today())

```



Gather Data for Currency Pairs - US Dollar and European Euro from 5/9/2019 until the value in cell D1

```

=GOOGLEFINANCE("CURRENCY:USDEUR","Price","5/9/2019",D1)


```


### ***Note***: For the best result, use reference cells in your formula to easily change the date and ticker as below:



![Google_Sheets_Data](Google_Sheets_Data.png)


[^1]: Here is [an example](https://docs.google.com/spreadsheets/d/1o_s3W20il3u-62fEhyoIMQFb3eignFwtVCyPga1fBwI/edit?usp=sharing) of the google sheet for reference. Make your copy, download it as CSV and start analysing now!
[^2]: [Link](https://support.google.com/docs/answer/3093281?hl=en) to official Google Finance Documents.

---