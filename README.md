# Amazon-Price-Checker
This is a web scraper built using BeautifulSoup Library.
Scrapes data from amazon product page and updates it at regular intervals - can be used to monitor price drops during sales and buy any product at it’s lowest price.

# Steps:
1. Took this amazon webpage : url = 'https://www.amazon.in/gp/aw/d/B0C3HD9KX5/?_encoding=UTF8&pd_rd_plhdr=t&aaxitk=33548c3715d3e04419b8a09135cd03ce&hsa_cr_id=0&qid=1697952223&sr=1-1-e0fa1fdd-d857-4087-adda-5bd576b25987&ref_=sbx_be_s_sparkle_mcd_asin_0_img&pd_rd_w=crFFI&content-id=amzn1.sym.df9fe057-524b-4172-ac34-9a1b3c4e647d%3Aamzn1.sym.df9fe057-524b-4172-ac34-9a1b3c4e647d&pf_rd_p=df9fe057-524b-4172-ac34-9a1b3c4e647d&pf_rd_r=4H8SV1PA0Y2M3S6C06KM&pd_rd_wg=VcBMI&pd_rd_r=768acc1f-30d3-489b-9bbe-f9e11017e0d0'
2. inspected the webpage to see the html code
3. Imported productTitle, price and rating attributes of the product page and also current date from datetime library to a csv file.
4. Created a price check function which apends productTitle, price, rating, date to the csv file for every 24hrs
5. We can keep this function running in the background of the system and view the prices whenever we want.
6. We can also add a condition in the price check function where if the price drops to certain amount we can get a mail about the price details and we can buy the product as per our budget.
7. We can add that mail part using smtp library
