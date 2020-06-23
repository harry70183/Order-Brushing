# Order-Brushing Detection
Brushing is a deceitful technique sometimes used in e-commerce to boost a seller's ratings by creating fake orders.  These fake orders, if unnoticed, can boost the seller's rating, which can make it more likely that their items will appear at the top of search results on e-commerce sites. To maintain the integrity of our oline shoppind experience, Shopee consistently monitor and flag any possible cases of order brushing on Shopee.
# Task
1. identify all shops that are deemed to have conducted order brushing.
2. For each shop that is identified to have conducted order brushing, identify the buyers suspected to have conducted order brushing for this shop.

For the purpose of this question, shops are deemed to have conducted order brushing if their concentrate rate is greater than or equal to 3 at any instance.

##Concentrate rate = number of Orders within 1 hour / number of unique buyer within 1 hour.

For the purpose of this question, suspicious buyers are deemed as the buyer that contributed the highest proportion of orders to a shop that is deemed to have conducted order brushing.

For the calculation of the highest proportion of orders to a shop, only include the orders that occured in instances when order brushing has been deemed to have taken place.

In the case where multiple users share the same highest proportion of orders for a specific shop, all those users are deemed to be suspicious buyers.

Please refer to the Examples.png for more specific cases of order brushing.

# Basic Concepts
Each orderid represents a distinct transcation on Shopee.

Each unique shopid is a distinct seller on Shopee.

Each unique userid is a distinct buyer on Shopee.

Event_Time refers to the exact time that an order was placed on Shopee.

Concentrate rate is a possible measure that we use to determine whether a shop is likely to have conducted order brushing. For this question, the thershold of concentrate rate is 3. Any concentrate rate value equal to or greater than 3 is deemed to be an occurance of order brushing.

# Submission Format

Check each shop and determine whether it is deemed to have conducted order brushing. If a shop conducted order brushing, list the userid(s) that are identified as suspicious for the corresponding shopid.

Two columns required:shopid, userid

- If a shop is not deemed to have conducted order brushing, assign the value 0.

- Else, list the userid(s) that are identified as suspicious for the corresponding shopid.

- If there is more than 1 userid identified as suspicious, list all the userids seperated by "&".
