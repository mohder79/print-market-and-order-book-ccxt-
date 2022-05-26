import ccxt  
from pprint import pprint
import api_config as ac

exchange = ccxt.bybit({
    'options': {
        'adjustForTimeDifference': True,
    },
    'apiKey': ac.API_KEY,
    'secret': ac.SECRET_KEY,
    'password': ac.PASSWORD,
})


print(exchange)


markets = exchange.load_markets()
pprint(markets)

symbol = 'BTC/USDT:USDT'
book = exchange.fetch_order_book(symbol)
pprint(book)
