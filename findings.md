First error I found was due to the get_temperature function using the wrong half
of the split() function.

I was able to then get to the sunscreen or moisturizer product page but got a
KeyError that broke the script. I knew that this is when you're referencing 
a key that's not in a dictionary. 

Since I got a positive result from the product type section but didn't even
get an error result from the "add products" section, I knew the problem
was occurring somewhere between there.

I figured it was in the purchase logic so I checked the e2e_weather_shopper_conf.py
file where conf is imported and found that the keys were not the same as what the
main program was referencing. 

I fixed that error and