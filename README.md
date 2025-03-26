# What does Expedia & Hotels.com Reviews Scraper do?
This **Apify Actor** helps you to **extract trusted reviews from any hotel, apartment or accommodation that is listed on [Expedia](https://euro.expedia.net/) and [Hotels.com](https://www.hotels.com/)**. To use it, simply **paste the URLs of your chosen hotel listings, click the 'Save & Start' button and instantly retrieve reviews** to help you choose the best hotel. It only works for **[Expedia](https://euro.expedia.net/)** and **[Hotels.com](https://www.hotels.com/)** sites and is not applicable for other booking portals. This tool is ideal for travelers who are searching for the most trustworthy and dependable hotel listing choices to choose from.

## What data can I extract from the Expedia & Hotels.com Reviews Scraper tool?
💯 Review **score, comment, date of submission and name of reviewer**  
👍 **Best hotel features** according to reviewers  
✅ Key **aspects/ themes that the reviewer valued**  
📅 **Duration and date** of reviewer's stay  
👪 **Type of traveler** (with a partner, family, group)

## Why should I scrape reviews from Expedia and Hotels.com?
✅ **Authentic Customer Feedback**: Gives you an overview of the satisfaction level of the reviewer by scraping from Expedia and Hotels.com websites.  
📈 **Market Analysis for Hotel Owners**: Advanced web scraping technologies enable the owners to conduct a research about their property and their competitors.  
🕜 **Time-efficient**: Extracts data from multiple platforms and combines them into one dataset which saves you from visiting multiple sites to collect data.  
💪 **Structured Data Results**: All scraped data is organized and converted into user-friendly formats such as CSV, Excel, JSON.  
🔗 **Integrate your Dataset**: Retrieve the data obtained from scraping Expedia and Booking.com reviews and integrate with our Apify API.

## How much will scraping reviews from Expedia and Hotels.com cost me?  
This [Actor](https://apify.com/tri_angle/expedia-hotels-com-reviews-scraper) calculates the pricing based on the number of results obtained. It will cost you **$1 to scrape 1,000 Expedia and Hotels.com reviews**. Plus, with the [Apify Free plan](https://apify.com/pricing), you can scrape upto **$5 of data for free each month**. To learn more about pricing, watch our video on [Apify pricing](https://www.youtube.com/watch?v=-wyz2iscZ30&ab_channel=Apify):  
https://www.youtube.com/watch?v=-wyz2iscZ30&ab_channel=Apify

## How to use the Expedia and Hotels.com Reviews Scraper?
Follow these quick simple steps to extract your dataset by using Expedia and Hotels.com Scraper:  
1. Use your email to create your [free Apify account](https://console.apify.com/sign-up).  
2. Open the required [Actor](https://console.apify.com/actors) on the Apify page and enter into your Apify console.  
3. Under the Input tab, **copy and paste the Expedia and Hotels.com URLs** that you would like to extract the reviews from.
4. You can also narrow down your search by **adding the maximum value for reviews per hotel, sorting out the ratings and adjusting the date of the written review**.  
5. Then click on the "Save & Start" button and your data is ready to be extracted!   
6. Once done, you can then obtain your results in **JSON, CSV, XML, Excel or HTML format**.
7. You can also connect the Apify API to integrate the [Expedia and Hotels.com Reviews Scraper](https://apify.com/tri_angle/expedia-hotels-com-reviews-scraper) with other cloud services such as **Google Drive, GitHub or any [other Apify Actors](https://docs.apify.com/platform/integrations)**. Follow this link to learn how to use the Apify API for scraping tasks: [Apify API Documentation](https://docs.apify.com/api/v2-redoc).  

## Input

The input for the Expedia and Hotels.com Reviews Scraper should contain the **URLs of either or both of Expedia and Hotels.com websites**. Here is an example of how the input will look like:  

```javascript  
{
    "minDate": "1990-01-01",
    "sortBy": "Most relevant",
    "startUrls": [
        {
            "url": "https://www.expedia.com/Prague-Hotels-Hotel-Krystal.h10966026.Hotel-Information",
            "method": "GET",
            "userData": {
                "hotel": "Prague Hotel Krystal",
                "doWeEndorseIt": "no opinion"
            }
        },
        {
            "url": "https://www.expedia.it/en/Berchtesgaden-Hotels-Alpensport-Hotel-Seimler.h2692552.Hotel-Information",
            "method": "GET",
            "userData": {
                "simple": false,
                "maxReviews": 100,
                "doWeEndorseThisHotel": "no opinion"
            }
        }
    ]
}
```  
The scraper allows you to configure certain properties which is explained in the [input tab](https://apify.com/tri_angle/expedia-hotels-com-reviews-scraper/input-schema).

## Output example  

The results of the runs are stored in the [Storage tab](https://console.apify.com/storage). You can either view your results in the form of a table in the Apify console, preview them in new tab or export them as an offline version. Here is a quick walkthrough on how you can access your output:
https://github.com/user-attachments/assets/175ed6fb-19a2-4f02-acc0-8c5c53a4b34d

Now you have an access to the list of reviews! Here are a few examples of reviews from the dataset in JSON:

```javascript  
[{
  "contentDirectFeedbackPromptId": null,
  "id": "657456105914715d6adf0fd1",
  "superlative": "Okay",
  "locale": "de_DE",
  "title": "Kein WiFi auf dem Zimmer",
  "brandType": "",
  "disclaimer": null,
  "reviewScoreWithDescription": {
    "label": "6 out of 10 Okay",
    "value": "6/10 Okay",
    "__typename": "LodgingEnrichedMessage"
  },
  "text": "Eigentlich ganz ok, schneller check in, Zimmer ok,  aaaber,\nkein WiFi auf den Zimmern und deshalb unbrauchbar und zu teuer. Zimmer ogne Internet ist nur die Hälfte wert. ",
  "highlightedText": null,
  "seeMoreAnalytics": {
    "linkName": "See more reviews",
    "referrerId": "HOT.HIS.See_more.",
    "__typename": "ClientSideAnalytics"
  },
  "submissionTime": {
    "longDateFormat": "Dec 9, 2023",
    "__typename": "DateTime"
  },
  "impressionAnalytics": null,
  "themes": [
    {
      "icon": {
        "id": "sentiment_4",
        "__typename": "Icon"
      },
      "label": "Liked: Cleanliness",
      "__typename": "ReviewThemes"
    },
    {
      "icon": {
        "id": "sentiment_2",
        "__typename": "Icon"
      },
      "label": "Disliked: Room comfort",
      "__typename": "ReviewThemes"
    }
  ],
  "reviewFooter": {
    "messages": [
      {
        "seoStructuredData": {
          "itemscope": true,
          "itemprop": "author",
          "itemtype": "https://schema.org/Person",
          "content": "Norbert",
          "__typename": "SEOStructuredData"
        },
        "text": {
          "text": "Stayed 3 nights in Dec 2023",
          "__typename": "EGDSPlainText"
        },
        "__typename": "PropertyReviewFooterMessage"
      }
    ],
    "__typename": "PropertyReviewFooterSection"
  },
  "reviewAnalytics": "{\"metadata\":{\"packer_version\":\"1.0.1\"},\"events\":{\"review.presented\":{\"v1\":{\"event_data\":{\"event\":{\"event_name\":\"review.presented\",\"event_version\":\"1.0.0\",\"event_type\":\"Impression\",\"action_location\":\"reviews_overlay\"},\"additional_context\":{\"user_interface\":{\"component_id\":\"657456105914715d6adf0fd1\",\"component_position\":21,\"component_name\":\"NEWEST_TO_OLDEST_BY_LANGUAGE.all\"}}}}}}}",
  "reviewInteractionSections": [
    {
      "primaryDisplayString": "0",
      "accessibilityLabel": "Mark review 1 as helpful. 0 other users found review 1 helpful.",
      "reviewInteractionType": "HELPFUL_REVIEW",
      "feedbackAnalytics": {
        "linkName": "Helpful review",
        "referrerId": "HOT.HIS.ReviewsOverlay.THUMB_UP.UPVOTE",
        "__typename": "ClientSideAnalytics"
      },
      "__typename": "PropertyReviewInteraction"
    },
    {
      "primaryDisplayString": null,
      "accessibilityLabel": null,
      "reviewInteractionType": "REVIEW_REPORT_FLAG",
      "feedbackAnalytics": null,
      "__typename": "PropertyReviewInteraction"
    },
    {
      "primaryDisplayString": "See more",
      "accessibilityLabel": "See more from Norbert's review",
      "reviewInteractionType": "REVIEW_EXPAND_LABEL",
      "feedbackAnalytics": null,
      "__typename": "PropertyReviewInteraction"
    },
    {
      "primaryDisplayString": "See less",
      "accessibilityLabel": "See less from Norbert's review",
      "reviewInteractionType": "REVIEW_COLLAPSE_LABEL",
      "feedbackAnalytics": null,
      "__typename": "PropertyReviewInteraction"
    }
  ],
  "__typename": "PropertyReview",
  "reviewAuthorAttribution": {
    "text": "Norbert",
    "__typename": "LodgingHeader"
  },
  "photoSection": null,
  "photos": [],
  "travelers": [],
  "translationInfo": {
    "loadingTranslationText": "Loading translation...",
    "targetLocale": null,
    "translatedBy": {
      "description": "Translated by Google",
      "__typename": "Mark"
    },
    "translationCallToActionLabel": "Translate with Google",
    "seeOriginalText": "See original",
    "__typename": "PropertyReviewTranslationInfo"
  },
  "propertyReviewSource": null,
  "reviewRegion": null,
  "managementResponses": [],
  "hotelId": "10966026",
  "reviewPosition": 21,
  "customData": {
    "hotel": "Prague Hotel Krystal",
    "doWeEndorseIt": "no opinion"
  }
},
{
  "contentDirectFeedbackPromptId": null,
  "id": "6535f83e0ee1f55b3a993c87",
  "superlative": "Excellent",
  "locale": "en_GB",
  "title": "",
  "brandType": "",
  "disclaimer": null,
  "reviewScoreWithDescription": {
    "label": "10 out of 10 Excellent",
    "value": "10/10 Excellent",
    "__typename": "LodgingEnrichedMessage"
  },
  "text": "",
  "highlightedText": null,
  "seeMoreAnalytics": {
    "linkName": "See more reviews",
    "referrerId": "HOT.HIS.See_more.",
    "__typename": "ClientSideAnalytics"
  },
  "submissionTime": {
    "longDateFormat": "Oct 23, 2023",
    "__typename": "DateTime"
  },
  "impressionAnalytics": null,
  "themes": null,
  "reviewFooter": {
    "messages": [
      {
        "seoStructuredData": {
          "itemscope": true,
          "itemprop": "author",
          "itemtype": "https://schema.org/Person",
          "content": "NIANGANE",
          "__typename": "SEOStructuredData"
        },
        "text": {
          "text": "Stayed 1 night in Oct 2023",
          "__typename": "EGDSPlainText"
        },
        "__typename": "PropertyReviewFooterMessage"
      }
    ],
    "__typename": "PropertyReviewFooterSection"
  },
  "reviewAnalytics": "{\"metadata\":{\"packer_version\":\"1.0.1\"},\"events\":{\"review.presented\":{\"v1\":{\"event_data\":{\"event\":{\"event_name\":\"review.presented\",\"event_version\":\"1.0.0\",\"event_type\":\"Impression\",\"action_location\":\"reviews_overlay\"},\"additional_context\":{\"user_interface\":{\"component_id\":\"6535f83e0ee1f55b3a993c87\",\"component_position\":22,\"component_name\":\"NEWEST_TO_OLDEST_BY_LANGUAGE.all\"}}}}}}}",
  "reviewInteractionSections": [
    {
      "primaryDisplayString": "0",
      "accessibilityLabel": "Mark review 2 as helpful. 0 other users found review 2 helpful.",
      "reviewInteractionType": "HELPFUL_REVIEW",
      "feedbackAnalytics": {
        "linkName": "Helpful review",
        "referrerId": "HOT.HIS.ReviewsOverlay.THUMB_UP.UPVOTE",
        "__typename": "ClientSideAnalytics"
      },
      "__typename": "PropertyReviewInteraction"
    },
    {
      "primaryDisplayString": "See more",
      "accessibilityLabel": "See more from NIANGANE's review",
      "reviewInteractionType": "REVIEW_EXPAND_LABEL",
      "feedbackAnalytics": null,
      "__typename": "PropertyReviewInteraction"
    },
    {
      "primaryDisplayString": "See less",
      "accessibilityLabel": "See less from NIANGANE's review",
      "reviewInteractionType": "REVIEW_COLLAPSE_LABEL",
      "feedbackAnalytics": null,
      "__typename": "PropertyReviewInteraction"
    }
  ],
  "__typename": "PropertyReview",
  "reviewAuthorAttribution": {
    "text": "NIANGANE",
    "__typename": "LodgingHeader"
  },
  "photoSection": null,
  "photos": [],
  "travelers": [],
  "translationInfo": null,
  "propertyReviewSource": null,
  "reviewRegion": null,
  "managementResponses": [],
  "hotelId": "10966026",
  "reviewPosition": 22,
  "customData": {
    "hotel": "Prague Hotel Krystal",
    "doWeEndorseIt": "no opinion"
  }
},

``` 
You can also export your data in other formats such as **CSV, Excel, HTML table or XML**.  

## What other online travel platforms can I scrape data from?  
If you would like to use some other travel platform to scrape data from, Apify also offers you a number of scrapers to choose from. You can retrieve various information such as hotel rankings, restaurant reviews and tourist attraction sites. Here are a few of them, feel free to explore more on Apify:  
|Platforms|Scraper links|  
|:--------|:------------|
|🦉 Tripadvisor| [Tripadvisor Scraper](https://apify.com/maxcopell/tripadvisor)|  
|📍 Google Maps| [Google Maps Reviews Scraper](https://apify.com/compass/google-maps-reviews-scraper)|  
|📘 Booking.com| [Booking Scraper](https://apify.com/voyager/booking-scraper)|  
|🅰️ Airbnb| [Airbnb Scraper](https://apify.com/tri_angle/airbnb-scraper)|  
|🌅 Skyscanner| [Skyscanner Flight](https://apify.com/jupri/skyscanner-flight)|  
|🛫 Ryanair| [Ryanair Scraper](https://apify.com/epctex/ryanair-scraper)|  

You can also have a look at similar Actor bundles such as [Hotel Review Aggregator](https://apify.com/tri_angle/hotel-review-aggregator), [Restaurant Review Aggregator](https://apify.com/tri_angle/restaurant-review-aggregator) and [Social Media Finder](https://apify.com/tri_angle/social-media-finder).

## ❓ FAQ

### Can I use the Expedia and Hotels.com Reviews Scraper with Apify API?  
The Apify API helps you to automate and manage Apify services using RESTful HTTP requests. You can run actors, retrieve data, schedule tasks and monitor progress by easily integrating it with Node.js by using `apify-client` NPM package and Python by using `apify-client` PyPI package.  

For more details, check out the [Apify API reference](https://docs.apify.com/api/v2) documentation and [API tab](https://apify.com/tri_angle/expedia-hotels-com-reviews-scraper/api/python) for code examples.

### Can I integrate Expedia and Hotels.com Reviews Scraper with other apps?  
Expedia and Hotels.com Reviews Scraper can be integrated with apps such as **Google Drive, GutHub, Keboola, Airbyte, Zapier, Make, LangChain, LlamaIndex, Flowise and [other Apify Actors](https://docs.apify.com/platform/integrations)**. You can find these [integrations](https://apify.com/integrations) on the Apify platform.  

You can also use [webhooks](https://docs.apify.com/platform/integrations/webhooks) to trigger notifications for different statuses, for instance, `ACTOR.RUN.CREATED` will notify you when a new Actor run has been created.

### Can I extract review data from Expedia and Hotels.com sites legally?
As long as the data is publicly available, it is possible to scrape reviews from Expedia and Hotels.com sites. It is however important to keep in mind certain legal guidelines:  
1. Only the reviews that are publicly visible to users without logging in are allowed to be collected.  
2. Given the fact that personal data is protected by GDPR in the European Union and by other comparable data protection laws worldwide, it is important to **respect the privacy policy and avoid scraping personal information such as names, emails or phone numbers**.  

It is highly recommended to seek legal counsel if you have questions regarding the legality of your data scraping. To learn more about legal scraping, check out our [blog post](https://blog.apify.com/is-web-scraping-legal/).

## Your feedback  
We are always working to make our Actors perform even better. You can use the Actor's [Issues tab](https://console.apify.com/actors/4zyibEJ79jE7VXIpA/issues?issueStatus=OPEN) if you spot a bug or have any technical feedback for us.
