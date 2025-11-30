# 🛍️ Bath & Body Works Product Scraper

![Bath & Body Works Product Scraper](https://i.ibb.co/V0Qbz16F/bath-bodyworks-cover.png)

This Apify actor scrapes product listings from the official [Bath & Body Works](https://www.bathandbodyworks.com/) website.  

<p align="center">
  <img src="https://apify-image-uploads-prod.s3.us-east-1.amazonaws.com/DevbkY3adMTBuoECt-actor-lafhMbu7OrUuDw3tl-j61TG2zEjz-images-8.png" alt="BathandBodyWorks Scraper" style="height: 60px; margin-right: 15px;" /><a href="https://apify.com/lexis-solutions/bath-and-body-works" target="_blank">
    <img src="https://img.shields.io/badge/Try%20it%20on-Apify-0066FF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDA4IiBoZWlnaHQ9IjQwOCIgdmlld0JveD0iMCAwIDQwOCA0MDgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxnIGNsaXAtcGF0aD0idXJsKCNjbGlwMF8zNDFfNDE1NykiPgo8cGF0aCBkPSJNMjE4LjY5NSAxMDRIMzAwLjk3QzMwMi42NDMgMTA0IDMwNCAxMDUuMzU3IDMwNCAxMDcuMDNWMjMyLjc2NkMzMDQgMjM1Ljc3OCAzMDAuMDgzIDIzNi45NDUgMjk4LjQzNCAyMzQuNDI1TDIxNi4xNTkgMTA4LjY5QzIxNC44NDEgMTA2LjY3NCAyMTYuMjg3IDEwNCAyMTguNjk1IDEwNFoiIGZpbGw9IndoaXRlIi8+CjxwYXRoIGQ9Ik0xODkuMzA1IDEwNEgxMDcuMDNDMTA1LjM1NyAxMDQgMTA0IDEwNS4zNTcgMTA0IDEwNy4wM1YyMzIuNzY2QzEwNCAyMzUuNzc4IDEwNy45MTcgMjM2Ljk0NSAxMDkuNTY2IDIzNC40MjVMMTkxLjg0IDEwOC42OUMxOTMuMTU5IDEwNi42NzQgMTkxLjcxMyAxMDQgMTg5LjMwNSAxMDRaIiBmaWxsPSJ3aGl0ZSIvPgo8cGF0aCBkPSJNMjAyLjU5MSAyMDQuNjY4TDEwOS4xMjcgMjk4LjgzNUMxMDcuMjI5IDMwMC43NDcgMTA4LjU4MyAzMDQgMTExLjI3OCAzMDRIMjk2LjhDMjk5LjQ4MyAzMDQgMzAwLjg0MiAzMDAuNzcgMjk4Ljk2NyAyOTguODUyTDIwNi45MDggMjA0LjY4NUMyMDUuNzI2IDIwMy40NzUgMjAzLjc4MiAyMDMuNDY4IDIwMi41OTEgMjA0LjY2OFoiIGZpbGw9IndoaXRlIi8+CjwvZz4KPGRlZnM+CjxjbGlwUGF0aCBpZD0iY2xpcDBfMzQxXzQxNTciPgo8cmVjdCB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEwNCAxMDQpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==&logoColor=white" alt="Try it on Apify" style="border-radius: 12px; height: 60px;" />
  </a>
</p>

You can fetch product data by using a keyword query or by selecting a specific category.

---


## 📊 Actor Stats

| Stat | Value |
|------|-------|
| **Version** | `0.0.3` |
| **Last Update** | Nov 30, 2025 |

---


## 🚀 Key Features

- **Flexible Search Options**: Scrape products by keyword or category.
- **Sorting Capabilities**: Sort results by best-sellers, new arrivals, price (low to high or high to low), or top-rated.
- **Result Limiting**: Limit the number of items retrieved using `maxItems`.
- **Proxy Support**: Uses Apify proxy configuration to avoid IP bans.

---

## 👤 Who Is This Actor Suitable For?

- **E-commerce Analysts** tracking competitor product listings and pricing.
- **Market Researchers** studying seasonal trends and product availability.
- **Developers** integrating product data into dashboards or databases.

---

## ❓ Why Use This Actor?

Manually collecting data from the Bath & Body Works website is time-consuming and error-prone.  
This actor automates the process and ensures you always get fresh, structured product data — fast and reliably.  
Ideal for competitive intelligence, monitoring promotions, or enriching product catalogs.

---

## Input Schema

```json
{
  "query": "candles", // query takes higher priority
  "category": "accessories",
  "sort": "best-sellers",
  "maxItems": 10,
  "proxyConfiguration": {
    "useApifyProxy": true
  }
}
```

## Output Schema

```json
{
  "currency": "USD",
  "id": "028011402",
  "imageGroups": [
    {
      "images": [
        {
          "alt": "Sweetest Song Fine Fragrance Mist",
          "disBaseLink": "https://www.bathandbodyworks.com/dw/image/v2/BBDL_PRD/on/demandware.static/-/Sites-master-catalog/default/dw0aa1b137/crop/028011402_crop.jpg",
          "link": "https://www.bathandbodyworks.com/on/demandware.static/-/Sites-master-catalog/default/dw0aa1b137/crop/028011402_crop.jpg",
          "title": "Sweetest Song Fine Fragrance Mist"
        }
      ],
      "viewType": "crop"
    },
    {
      "images": [
        {
          "alt": "Sweetest Song Fine Fragrance Mist",
          "disBaseLink": "https://www.bathandbodyworks.com/dw/image/v2/BBDL_PRD/on/demandware.static/-/Sites-master-catalog/default/dw3ef8d056/hires/028011402.jpg",
          "link": "https://www.bathandbodyworks.com/on/demandware.static/-/Sites-master-catalog/default/dw3ef8d056/hires/028011402.jpg",
          "title": "Sweetest Song Fine Fragrance Mist"
        },
        {
          "alt": "Sweetest Song Fine Fragrance Mist",
          "disBaseLink": "https://www.bathandbodyworks.com/dw/image/v2/BBDL_PRD/on/demandware.static/-/Sites-master-catalog/default/dw0054ab5e/hires/028011402_alt_1.jpg",
          "link": "https://www.bathandbodyworks.com/on/demandware.static/-/Sites-master-catalog/default/dw0054ab5e/hires/028011402_alt_1.jpg",
          "title": "Sweetest Song Fine Fragrance Mist"
        }
      ],
      "viewType": "hires"
    }
  ],
  "inventory": {
    "ats": 82550,
    "backorderable": false,
    "id": "inventory-bb2na-bb2us",
    "orderable": true,
    "preorderable": false,
    "stockLevel": 82550
  },
  "longDescription": "<p>What it does: scents your skin with a mist that's super layerable.</p>\n\n<p>Why you'll love it:</p><ul class=\"pdp_ov_ul\">\n<li>The truest way to fragrance</li>\n<li>Designed for great coverage</li>\n<li>Made without parabens</li>\n<li>Dermatologist tested</li></ul>",
  "minOrderQuantity": 1,
  "name": "Sweetest Song Fine Fragrance Mist",
  "price": 18.95,
  "pricePerUnit": 18.95,
  "prices": {
    "usd-list-prices": 18.95
  },
  "primaryCategoryId": "body-sprays-mists",
  "productPromotions": [
    {
      "calloutMsg": "Mix & Match: B3G1",
      "promotionId": "TBC_b3g1_clone"
    },
    {
      "promotionId": "PWP_MothersDay_45w40Purch"
    }
  ],
  "shortDescription": "<p>What it smells like: music that takes you back to the best day ever.</p>\n\n<p>What it does: nourishes your skin for the most refreshing, truest way to fragrance.</p>",
  "slugUrl": "https://www.bathandbodyworks.com/p/sweetest-song-fine-fragrance-mist-028011402.html",
  "stepQuantity": 1,
  "type": {
    "item": true
  },
  "upc": "667659345700",
  "validFrom": {
    "default": "2025-03-13T10:00:00.000Z"
  },
  "c_MSRP": 18.95,
  "c_SearchBoostKeyword": "coquette",
  "c_autoRefresh": false,
  "c_availableForInStorePickup": true,
  "c_bvAverageRating": "4.6979",
  "c_bvRatingRange": "5",
  "c_bvReviewCount": "854",
  "c_class": 201,
  "c_className": "SC CORE",
  "c_clearance": true,
  "c_collection": "SFL",
  "c_color": "Pink",
  "c_countryOfOrigin": "US",
  "c_daysSinceLaunch": 68,
  "c_dept": 51,
  "c_deptName": "SIGNATURE COLLECTION",
  "c_form": "Fine Fragrance Mist",
  "c_fragranceCategories": ["Floral", "Fruity"],
  "c_fragranceCategory": "Fruity",
  "c_fragranceDescription": "<p>What it smells like: music that takes you back to the best day ever.</p>\n\n<p>Fragrance notes: blush raspberries, sugar crystals and whipped musk.</p>",
  "c_fragranceName": "Sweetest Song",
  "c_hasILNAssociation": true,
  "c_hazmatCode": "9E",
  "c_hideFromSearch": "NO",
  "c_holidaysCelebrations": ["Bridal Shower", "Gifts for Her", "Spring"],
  "c_launchDate": "2025-03-13T10:00:00.000Z",
  "c_maxOrderable": 25,
  "c_olfactiveSpace": "Fruity & Bright",
  "c_productBadge": "New Fragrance",
  "c_productSent": false,
  "c_productType": "Body Spray & Mist",
  "c_sapCategoryCode": "3002",
  "c_sapCategoryDesc": "FRAGRANCE-PCB",
  "c_sapClassCode": "40020007",
  "c_sapClassDesc": "JUICE-FRAGRANCE",
  "c_sapCollection": "N/A",
  "c_sapSectorCode": "201",
  "c_sapSectorDesc": "PERSONALCARE+BEAUTY",
  "c_sapSubbrandCode": "1612",
  "c_sapSubbrandDesc": "SIGNATURE",
  "c_sapSubclassCode": "1916",
  "c_sapSubclassDesc": "MIST/SPLASH - JUICE",
  "c_size": "8 fl oz / 236 mL",
  "c_sortPrice": 18.95,
  "c_subclass": 215,
  "c_subclassName": "SC FRAGRANCE MIST",
  "c_theme": "SP3 - 2025",
  "c_productName": "Sweetest Song",
  "c_listPrice": "18.95",
  "c_purchaseLimit": {
    "categoryLimit": 10000,
    "webLimit": 25
  },
  "c_forceSoldOut": false,
  "primaryImageUrl": "https://www.bathandbodyworks.com/on/demandware.static/-/Sites-master-catalog/default/dw0aa1b137/crop/028011402_crop.jpg"
}
```

---

## 🔍 Looking to Scrape Other Shopping Websites?

In addition to this actor, you can explore our suite of dedicated scrapers tailored for other popular e-commerce platforms. Each scraper is optimized for its target site to ensure accurate, efficient, and high-performance data extraction.

| Scraper                                                                                | Description                                                                                                          |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| [Notino Scraper](https://apify.com/lexis-solutions/notino-scraper)                     | Extract product details, prices, and availability from Notino's extensive catalog of beauty and personal care items. |
| [Capital One Shopping Scraper](https://apify.com/lexis-solutions/capital-one-shopping) | Gather shopping deals and offers directly from CapitalOneShopping.com.                                               |
| [Michaels Scraper](https://apify.com/lexis-solutions/michaels-scraper)                 | Retrieve product listings, categories, and pricing from the Michaels craft store website.                            |

Explore these solutions to expand your data collection capabilities across different retail websites.

---

👀 p.s.

Got feedback or need an extension?

Lexis Solutions is a [certified Apify Partner](https://apify.com/partners/find). We can help you with custom solutions or data extraction projects.

Contact us over [Email](mailto:scraping@lexis.solutions) or [LinkedIn](https://www.linkedin.com/company/lexis-solutions)

## Support Our Work 💝

If you're happy with our work and scrapers, you're welcome to leave us a company review [here](https://apify.com/partners/find/lexis-solutions/review) and leave a review for the scrapers you're subscribed to. It will take you less than a minute but it will mean a lot to us!

Image Credit: https://www.bathandbodyworks.com/
