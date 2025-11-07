# Pricing American options with binomial trees

This is my project submitted for the Fall 2025 Quant Finance course at Erdos Institute.

Goals:
* Explore the different aspects of American vs European options. As American options can be exercised before the expiration time, Black-Sholes does not yield the closed form for call/put option pricing.
* Realize some of the standard and well-known binomial models: CRR (Cox-Ross-Rubinstein), JR (Jarrow-Rudd) and Tian binomial tree models.
* Test the implementations using the yfinance data.

As a result, we have impelemented the following procedures:

```python 
def american_option_price_call_CRR(S0, K, T, r, sigma, n):
    """
    Computes the price of an American option using the CRR binomial model.

    Args:
        S0 (float): Initial stock price.
        K (float): Strike price.
        T (float): Time to maturity in years.
        r (float): Risk-free interest rate.
        sigma (float): Volatility of the underlying asset.
        n (int): Number of steps in the binomial tree.
    Returns:
        float: The calculated American option price.
    """
def american_option_price_put_CRR(S0, K, T, r, sigma, n):
    """
    Computes the price of an American option using the CRR binomial model.

    Args:
        S0 (float): Initial stock price.
        K (float): Strike price.
        T (float): Time to maturity in years.
        r (float): Risk-free interest rate.
        sigma (float): Volatility of the underlying asset.
        n (int): Number of steps in the binomial tree.
    Returns:
        float: The calculated American option price.
    """

def tian_american_binomial_call(S0, K, T, r, sigma, n):
    """
    Prices an American-style option using the Tian (1993) binomial model.

    Parameters:
    - S0: float, Current stock price
    - K: float, Strike price
    - T: float, Time to maturity (in years)
    - r: float, Risk-free interest rate (annualized, continuous)
    - sigma: float, Volatility (annualized)
    - n: int, Number of time steps in the binomial tree
    - option_type: str, 'call' or 'put'

    Returns:
    - float: The estimated price of the American option
    """
def tian_american_binomial_put(S0, K, T, r, sigma, n):
    """
    Prices an American-style option using the Tian (1993) binomial model.

    Parameters:
    - S0: float, Current stock price
    - K: float, Strike price
    - T: float, Time to maturity (in years)
    - r: float, Risk-free interest rate (annualized, continuous)
    - sigma: float, Volatility (annualized)
    - n: int, Number of time steps in the binomial tree
    - option_type: str, 'call' or 'put'

    Returns:
    - float: The estimated price of the American option
    """

def jarrow_rudd_american_binomial_call(S0, K, T, r, sigma, N):
    """
    Prices an American-style option using the Jarrow-Rudd (1983) binomial model.

    Parameters:
    - S0: float, Current stock price
    - K: float, Strike price
    - T: float, Time to maturity (in years)
    - r: float, Risk-free interest rate (annualized, continuous)
    - sigma: float, Volatility (annualized)
    - N: int, Number of time steps in the binomial tree
    - option_type: str, 'call' or 'put'

    Returns:
    - float: The estimated price of the American option
    """

def jarrow_rudd_american_binomial_put(S0, K, T, r, sigma, N):
    """
    Prices an American-style option using the Jarrow-Rudd (1983) binomial model.

    Parameters:
    - S0: float, Current stock price
    - K: float, Strike price
    - T: float, Time to maturity (in years)
    - r: float, Risk-free interest rate (annualized, continuous)
    - sigma: float, Volatility (annualized)
    - N: int, Number of time steps in the binomial tree
    - option_type: str, 'call' or 'put'

    Returns:
    - float: The estimated price of the American option
    """

def get_options_run_model(ticker_name="AAPL", start='2025-11-01', end='2025-11-05', interval='1m', r=0.03, expiration_date='2025-11-07', model="CRR", option_type="call"):
    """
    Fetches the option data for the given ticker and given dates, outputs the graph which shows 
    the relation between the yfinance prices and modeled prices using one of the binomial tree models implemented.
    ticker_name: Stock ticker
    start: Starting date
    end: Final date
    interval: The interval between distinct stock prices
    r: Interest rate
    expiration_date: Expiration date
    model = Can be 'CRR' or 'JR' or 'Tian'
    option type: 'call' or 'put'
    """

```
## TODO:

Nice things to do in the future:
* Realize option pricing schemes using Levy processes
* Obtain more data for stocks on other non-US based exchanges?


