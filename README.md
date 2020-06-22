# Order-Brushing Detection
Brushing is a deceitful technique sometimes used in e-commerce to boost a seller's ratings by creating fake orders.  These fake orders, if unnoticed, can boost the seller's rating, which can make it more likely that their items will appear at the top of search results on e-commerce sites. To maintain the integrity of our oline shoppind experience, Shopee consistently monitor and flag any possible cases of order brushing on Shopee.
# Task
1. identify all shops that are deemed to have conducted order brushing.
2. For each shop that is identified to have conducted order brushing, identify the buyers suspected to have conducted order brushing for this shop.

For the purpose of this question, shops are deemed to have conducted order brushing if their concentrate rate is greater than or equal to 3 at any instance.

##Concentrate rate = number of Orders within 1 hour / number of unique buyer within 1 hour.

For the purpose of this question, suspicious buyers are deemed as the buyer that contributed the highest proportion of orders to a shop that is deemed to have conducted order brushing.
For the calculation of the highest proportion of orders to a shop, only include the orders that occured in instances when order brushing has been deemed to have taken place.
In the case where multiple users share the same highest proportion
