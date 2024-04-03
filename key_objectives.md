

# Key Objectives
---

1. Evaluate **product performance** based on sales data, consumer ratings, and pricing information.
    - Here, available features are `selling_price` and `original_price`, discount offered can be compared with ratings and reviews
    
    \
    New feature **can be** added as `discount_offered`

    ```discount_offered = 100 * (original_price - selling_price)/original_price```
    
    \
        - more `discount_offered` less `customer_reviews_count` with good `product_rating` $\implies$ product needs marketing
        
        \
        - more `customer_reviews_count` with good `product_rating` $\implies$ product is performing great and no need to offer discount

\
2. Identify **trends and patterns within product categories** to uncover high-demand items and growth opportunities.
    - Indirect demand **can be** defined depending upon

    <figure>

        <span style="color:blue">table 01</span>

        <img src="https://drive.google.com/uc?id=1eTMSxARYh23TAUusP8jGtRZT7UojS5eg" height=130>
    </figure>

3. Assess **brand performance** to understand brand loyalty and market share.
    - brands with more # of demanding products can be tracked

    - Market share **can be** tracked by tabulating `brand` vs `category`,

    \
    for e.g. `category = "Baby Care"` has total
$65$ brands contributing to $610$ products
    
    here, `threshold` is set as `20`, brands having less than
$20$ products combined as `local brand`  

    <img  src="https://drive.google.com/uc?id=1qTEFtmRYOy2Kw1EHfNOa0k7qGEORaRa5" alt="[650 x 1080]" height=650 width = 1080>
    

\
4. Analyze the **relationship between pricing strategies and consumer perception** to optimize pricing.
    - *highly discounted* products may be percieved as *not so worthy*
    
    - find products with **low** `customer_review_count` with **good** `product_rating` (refer `table 01`)

        - for such products more discount can be offered with marketing, so as to gain popularity for the product

\
5. Explore consumer feedback/ratings to gain insights into **preferences and satisfaction levels across product categories.**

    - following data is just intiutivly tabulated (needs to dig deeper)
    
    <img src="https://drive.google.com/uc?id=1uwlL3G33G2e0CXhbl8Yms52J_7xum0Cw" alt="[400xY]" height=300>

    - Imputation can be done taking **median** across `brand`

\
6. **Compare product performance metrics with competitors** to identify strengths, weaknesses, and opportunities for improvement.

    - Align with objective 1 with **groupby brand**