[Instagram Comment Scraper](https://apify.com/scraptivo/instagram-comment-scraper?fpr=data)

Extract all comments from Instagram posts/reels with just the URL. Get usernames, profile images, comment text, likes, reply counts, and dates — perfect for research, sentiment analysis, or influencer insights.

Features

- Extract all comments

- Image
- Username
- Name
- Post/Reel URL
- Comment
- Likes
- Reply Count
- Date of Comment
- Supports proxies for anonymity and bypassing restrictions.
- Fast and reliable scraping with retry mechanisms.

## Pricing

```
- $10/1000 comments
- No hidden fees or limits on usage.
```

---

## Input

The actor accepts the following input:

- **post_urls** (list(string), required): Post URLs to get the comments from
- **posts_concurrency** (int, optional): Number of posts to processing at a time
- **proxyConfiguration** (object, optional): Proxy settings for enhanced scraping

### 📝 Copy for Use:

```
{
  "post_urls": [
    "https://www.instagram.com/p/DWte0fylh5b/"
  ],
  "proxyConfiguration": {
    "useApifyProxy": true,
    "apifyProxyGroups": [
      "RESIDENTIAL"
    ],
    "apifyProxyCountry": "US"
  },
  "posts_concurrency": 2,
  "sleep_min": 5,
  "sleep_max": 12,
  "request_timeout": 120,
  "request_retries": 1,
  "rate_limit_cooldown": 300,
  "rate_limit_max_waits": 3
}
```

---

## Why Choose This Scraper?

- **Affordable**: Pay only $10 per 1,000 products scraped
- **Comprehensive**: Extracts all essential product details including pricing and stock levels
- **Easy to Use**: Simple setup and integration with the Apify platform
- **Reliable**: Built with retry mechanisms to handle network issues
- **Location-aware**: Get accurate pricing and availability for specific delivery locations

---

## Recommended Proxy Providers

- ## **Shifter**

- Reliable residential proxies all over the world.
- Cheap rates
- [Order Shifter Now](https://shifter.io/r/YoBB/order)
- Get 10% Off any product, use coupan `rigelbytes-YoBB`.
- ## **OxyLabs**

- **100M+ Proxies**
- Fastest proxies in the market
- Real profile, human-like Residential IPs
- Quality assurance framework for most reliable IPs
- [Get Proxies](https://oxylabs.go2cloud.org/aff_c?offer_id=7&aff_id=1366&url_id=7)
- ## **DataImpulse**

- Covers **200+ Counties**
- Reliable Residential Proxies for just $1/GB
- [Get Residential Proxies](https://dataimpulse.com/?aff=89421)

## ![Learn More About Proxies](https://img.shields.io/badge/Learn_More-About_Proxies-blue?style=for-the-badge)

## 🙌 Why Buy Through Our Affiliate Link?

- Exclusive Deals: Some providers may offer special discounts or bonuses when you use our link.
- Support Our Work: Each purchase helps us maintain and improve the tools and services we provide.
- No Extra Cost: You pay the same price, but part of it goes to supporting our efforts.

### Running via Apify Console

You can run this actor from the Apify Console by providing the necessary input parameters.

### Running via API

You can trigger this actor using the Apify API, passing the required input in the request body.

## API Request Example (Python)

```
from apify_client import ApifyClient

# Initialize the ApifyClient with your API token
client = ApifyClient("<YOUR_API_TOKEN>")

# Prepare the Actor input
run_input = {
  "post_urls": [
    "https://www.instagram.com/p/DWte0fylh5b/"
  ],
  "proxyConfiguration": {
    "useApifyProxy": true,
    "apifyProxyGroups": [
      "RESIDENTIAL"
    ],
    "apifyProxyCountry": "US"
  },
  "posts_concurrency": 2,
  "sleep_min": 5,
  "sleep_max": 12,
  "request_timeout": 120,
  "request_retries": 1,
  "rate_limit_cooldown": 300,
  "rate_limit_max_waits": 3
}

# Run the Actor and wait for it to finish
run = client.actor("rigelbytes/rigelbytes/instagram-comment-scraper").call(run_input=run_input)
```

## JavaScript

```
import { ApifyClient } from 'apify-client';

// Initialize the ApifyClient with your API token
const client = new ApifyClient({
    token: '<YOUR_API_TOKEN>',
});

// Prepare Actor input
const input = {
  "post_urls": [
    "https://www.instagram.com/p/DWte0fylh5b/"
  ],
  "proxyConfiguration": {
    "useApifyProxy": true,
    "apifyProxyGroups": [
      "RESIDENTIAL"
    ],
    "apifyProxyCountry": "US"
  },
  "posts_concurrency": 2,
  "sleep_min": 5,
  "sleep_max": 12,
  "request_timeout": 120,
  "request_retries": 1,
  "rate_limit_cooldown": 300,
  "rate_limit_max_waits": 3
};

(async () => {
    // Run the Actor and wait for it to finish
    const run = await client.actor("rigelbytes/rigelbytes/instagram-comment-scraper").call(input);
})();
```

## Running with cURL

```
# Set API token
API_TOKEN=<YOUR_API_TOKEN>

# Prepare Actor input
cat > input.json <<'EOF'
{
  "post_urls": [
    "https://www.instagram.com/p/DWte0fylh5b/"
  ],
  "proxyConfiguration": {
    "useApifyProxy": true,
    "apifyProxyGroups": [
      "RESIDENTIAL"
    ],
    "apifyProxyCountry": "US"
  },
  "posts_concurrency": 2,
  "sleep_min": 5,
  "sleep_max": 12,
  "request_timeout": 120,
  "request_retries": 1,
  "rate_limit_cooldown": 300,
  "rate_limit_max_waits": 3
}
EOF

# Run the Actor
curl "https://api.apify.com/v2/acts/rigelbytes/rigelbytes/instagram-comment-scraper/runs?token=$API_TOKEN" \
  -X POST \
  -d @input.json \
  -H 'Content-Type: application/json'
```

- ## Output

![Output](https://images.apifyusercontent.com/yQTRxOIS3I8KZIhJHbkuzSrIZzf0UdBLniE4kDDPh88/w:1800/cb:1/aHR0cHM6Ly9yYXcuZ2l0aHVidXNlcmNvbnRlbnQuY29tL2ZhaXphbmFsaWkvYXBpZnktaW1hZ2VzLzk3MjYzZDUwOTBlNDYzNjU0NzRhZTRkZDNmMzJiZGZkNTg1MzBmODMvaW5zdGFncmFtLWNvbW1lbnQtc2NyYXBlci5naWY.webp)

## ![View Detailed Data](https://img.shields.io/badge/Detailed-Data-green?style=for-the-badge)

## 🚀 Other Tools by Rigel Bytes

[![Airbnb Images Downloader](https://img.shields.io/badge/Airbnb_Images_Downloader-blue?style=for-the-badge)](https://apify.com/rigelbytes/airbnb-images-downloader)

A focused Airbnb image scraper that extracts all photos from an Airbnb listing page and packages the listing's image files into a compressed archive. The Act...

[![Zillow Scraper](https://img.shields.io/badge/Zillow_Scraper-green?style=for-the-badge)](https://apify.com/rigelbytes/zillow-scraper)

A Zillow-focused web scraper that extracts structured property listing data for real estate analysis and monitoring. The Actor crawls Zillow listings to coll...

[![Zillow Detail Scraper](https://img.shields.io/badge/Zillow_Detail_Scraper-orange?style=for-the-badge)](https://apify.com/rigelbytes/zillow-detail-scraper)

Zillow scraper with customizable proxy support. Extract comprehensive property data, including pricing, images, and location details, using your proxies for better control and efficiency. Check the recommended proxy providers below.

[![Daraz](https://img.shields.io/badge/Daraz-blueviolet?style=for-the-badge)](https://apify.com/rigelbytes/daraz)

A web scraping Actor that extracts product listings and detailed product and seller data from Daraz.pk (Pakistan ecommerce marketplace) for monitoring and an...

[![Airbnb Listing](https://img.shields.io/badge/Airbnb_Listing-red?style=for-the-badge)](https://apify.com/rigelbytes/airbnb-listing)

A web-scraping Actor that bulk-extracts structured Airbnb listing data from listing pages: it retrieves listing metadata, descriptive content, property featu...

[![Google Maps Scraper](https://img.shields.io/badge/Google_Maps_Scraper-yellow?style=for-the-badge)](https://apify.com/rigelbytes/google-maps-scraper)

A Google Maps scraping Actor that extracts structured business profiles and local place intelligence at scale: it crawls Google Maps listings to collect busi...

[![Airbnb Availability Calendar](https://img.shields.io/badge/Airbnb_Availability_Calendar-purple?style=for-the-badge)](https://apify.com/rigelbytes/airbnb-availability-calendar)

Exports Airbnb listing availability calendars by scraping listing pages and producing structured, per-date calendar data. The Actor extracts date entries and...

[![Instagram Profile Scraper](https://img.shields.io/badge/Instagram_Profile_Scraper-pink?style=for-the-badge)](https://apify.com/rigelbytes/instagram-profile-scraper)

A web-scraping Actor that extracts detailed Instagram profile and media metadata from profile pages: it retrieves profile-level metrics (follower/following c...

[![Land.com Scraper](https://img.shields.io/badge/Land.Com_Scraper-cyan?style=for-the-badge)](https://apify.com/rigelbytes/landdotcom-scraper)

A Land.com-focused web scraper that crawls Land.com property listings and extracts structured real estate data for specified geographic areas and listing typ...

[![Airbnb Reviews](https://img.shields.io/badge/Airbnb_Reviews-success?style=for-the-badge)](https://apify.com/rigelbytes/airbnb-reviews)

A web-scraping Actor that extracts unlimited reviews from Airbnb listings: it crawls listing review pages and produces structured review records containing r...

[![FurnishedFinder](https://img.shields.io/badge/Furnishedfinder-important?style=for-the-badge)](https://apify.com/rigelbytes/furnishedfinder)

A web-scraping Actor designed to extract large-scale furnished rental data from Furnished Finder: it crawls listing pages to collect listing metadata (proper...

[![Immobilienscout24](https://img.shields.io/badge/Immobilienscout24-critical?style=for-the-badge)](https://apify.com/rigelbytes/immobilienscout24)

A scraper for immobilienscout24.de that extracts large-scale real estate listing data and contact information, optimized for bulk property data collection, i...

[![Airbnb Listing Urls](https://img.shields.io/badge/Airbnb_Listing_Urls-informational?style=for-the-badge)](https://apify.com/rigelbytes/airbnb-listing-urls)

A web scraper that extracts unlimited Airbnb listings from search queries and returns structured listing metadata for analysis. The Actor crawls Airbnb searc...

[![Instagram Engagement Tool](https://img.shields.io/badge/Instagram_Engagement_Tool-9cf?style=for-the-badge)](https://apify.com/rigelbytes/instagram-engagement-tool)

Analyzes public Instagram profiles by scraping recent posts and profile metadata to compute engagement metrics for images and videos. The Actor extracts prof...

[![Instagram Post Scraper](https://img.shields.io/badge/Instagram_Post_Scraper-blue?style=for-the-badge)](https://apify.com/rigelbytes/instagram-post-scraper)

An Instagram scraping Actor that extracts every post from Instagram profiles and produces structured post-level metadata and media assets for social media an...

[![BBB Scraper](https://img.shields.io/badge/Bbb_Scraper-green?style=for-the-badge)](https://apify.com/rigelbytes/bbb-scraper)

A web-scraping Actor that extracts detailed business listings from the Better Business Bureau (BBB). It crawls BBB listings and produces structured business ...

[![Linkedin Company Scraper](https://img.shields.io/badge/Linkedin_Company_Scraper-orange?style=for-the-badge)](https://apify.com/rigelbytes/linkedin-company-scraper)

A LinkedIn Company Scraper that extracts structured company profile data from LinkedIn company pages for lead generation and competitive intelligence. The Ac...

[![linkedin-company-details](https://img.shields.io/badge/Linkedin_Company_Details-blueviolet?style=for-the-badge)](https://apify.com/rigelbytes/linkedin-company-details)

A LinkedIn Company Scraper for extracting comprehensive company profiles and social content from LinkedIn: it scrapes and returns structured company profile ...

[![Instagram Reel Scraper](https://img.shields.io/badge/Instagram_Reel_Scraper-red?style=for-the-badge)](https://apify.com/rigelbytes/instagram-reel-scraper)

A web-scraping Actor that extracts all Instagram Reels from public profiles and produces structured reel-level metadata for content analysis, research, and m...

[![Rottentomatoes Reviews Scraper](https://img.shields.io/badge/Rottentomatoes_Reviews_Scraper-yellow?style=for-the-badge)](https://apify.com/rigelbytes/rottentomatoes-reviews-scraper)

A web-scraping Apify Actor that extracts user and critic reviews from Rotten Tomatoes pages, producing structured review records for analysis. It crawls unli...

[![Extract Furnished Finder Hosts](https://img.shields.io/badge/Extract_Furnished_Finder_Hosts-purple?style=for-the-badge)](https://apify.com/rigelbytes/furnished-finder-hosts)

Scrapes Furnished Finder listings and extracts structured listing and host profile data for furnished rentals, including listing titles, property types, geol...

[![Trustpilot Reviews Scraper](https://img.shields.io/badge/Trustpilot_Reviews_Scraper-pink?style=for-the-badge)](https://apify.com/rigelbytes/trustpilot-reviews)

A Trustpilot review scraper that collects structured review records and full reviewer profile data at scale. It extracts review content (titles and body text...

[![Furnished Finder Fast](https://img.shields.io/badge/Furnished_Finder_Fast-cyan?style=for-the-badge)](https://apify.com/rigelbytes/furnished-finder-fast)

An Apify Actor for scraping Furnished Finder rental listings and optional host profiles, extracting structured listing data such as photos, textual descripti...

[![Zillow Agents](https://img.shields.io/badge/Zillow_Agents-success?style=for-the-badge)](https://apify.com/rigelbytes/zillow-agents)

A Zillow agent profile scraper that extracts structured agent data from Zillow for location-based queries (city, neighborhood, ZIP). The Actor scrapes agent ...

[![Bayut Scraper](https://img.shields.io/badge/Bayut_Scraper-important?style=for-the-badge)](https://apify.com/rigelbytes/bayut-scraper)

A web-scraping Actor for extracting structured property listings and market intelligence from Bayut.com (UAE). It crawls Bayut property pages and returns str...

[![dubai-listing-scraper](https://img.shields.io/badge/Dubai_Listing_Scraper-critical?style=for-the-badge)](https://apify.com/rigelbytes/dubai-listing-scraper)

A web scraping Actor for Bayut.com that extracts structured UAE property listing data for sale and rent across Dubai, Abu Dhabi and other Emirates. It progra...

[![Tiktok Comment Scraper](https://img.shields.io/badge/Tiktok_Comment_Scraper-informational?style=for-the-badge)](https://apify.com/rigelbytes/tiktok-comment-scraper)

A TikTok comment scraping Actor that extracts all comments from TikTok videos given a video URL. It collects commenter metadata (usernames, display names, pr...

[![Tiktok Engagement Rate](https://img.shields.io/badge/Tiktok_Engagement_Rate-9cf?style=for-the-badge)](https://apify.com/rigelbytes/tiktok-engagement-rate)

A TikTok profile scraper that analyzes public TikTok accounts to extract profile metadata and recent video-level interaction metrics and to compute engagemen...

[![Company Service Finder](https://img.shields.io/badge/Company_Service_Finder-blue?style=for-the-badge)](https://apify.com/rigelbytes/company-service-finder)

Company Service Finder scrapes business listings from Google Search and Google Maps across cities and states, extracts company websites, names, phone numbers...

[![Website Services Finder](https://img.shields.io/badge/Website_Services_Finder-green?style=for-the-badge)](https://apify.com/rigelbytes/website-services-finder)

Website Services Finder extracts and AI-analyzes company services and business information from business websites using web crawling plus large-language and ...

[![Airbnb Address Finder](https://img.shields.io/badge/Airbnb_Address_Finder-orange?style=for-the-badge)](https://apify.com/rigelbytes/airbnb-address-finder)

A web-scraping Apify Actor that bulk-extracts Airbnb listing addresses and comprehensive listing metadata from provided Airbnb listing URLs. It parses listin...

[![Immowelt Scraper](https://img.shields.io/badge/Immowelt_Scraper-blueviolet?style=for-the-badge)](https://apify.com/rigelbytes/immowelt-scraper)

An Apify Actor that scrapes unlimited real estate listings from immowelt.de and returns structured property data for indexing and analysis. The Actor extract...

[![Propertyfinder Scraper](https://img.shields.io/badge/Propertyfinder_Scraper-red?style=for-the-badge)](https://apify.com/rigelbytes/propertyfinder-scraper)

A scraper for propertyfinder.ae that extracts unlimited real estate listings and related metadata at scale. Implements asynchronous concurrency, automatic re...

[![Publix Scraper](https://img.shields.io/badge/Publix_Scraper-yellow?style=for-the-badge)](https://apify.com/rigelbytes/publix-scraper)

A web scraping Actor for Publix.com that extracts grocery product data from Publix collection pages using a collection URL and a delivery/pickup location to ...

[![Redfin Scraper](https://img.shields.io/badge/Redfin_Scraper-purple?style=for-the-badge)](https://apify.com/rigelbytes/redfin-scraper)

Redfin Scraper extracts large-scale real estate listing data from Redfin search and city pages and returns structured property records for downstream analysi...

[![Instacart Scraper](https://img.shields.io/badge/Instacart_Scraper-pink?style=for-the-badge)](https://apify.com/rigelbytes/instacart-scraper)

A web-scraping Actor that extracts structured product data from instacart.com using a collection/search keyword combined with a delivery or pickup location; ...

[![Homedepot Scraper](https://img.shields.io/badge/Homedepot_Scraper-cyan?style=for-the-badge)](https://apify.com/rigelbytes/homedepot-scraper)

A web scraper for homedepot.com that crawls collection pages and performs location-aware scraping (delivery or pickup) to extract structured product data. Th...

[![Doctify Scraper](https://img.shields.io/badge/Doctify_Scraper-success?style=for-the-badge)](https://apify.com/rigelbytes/doctify-scraper)

A web scraping Actor that extracts structured healthcare provider and practice data from doctify.com starting from a Doctify search-results URL. The Actor ha...

[![Facebook Ads Scraper](https://img.shields.io/badge/Facebook_Ads_Scraper-important?style=for-the-badge)](https://apify.com/rigelbytes/facebook-ads-scraper)

Extracts structured ad data from the Facebook Ads Library using a search URL: scrapes ad metadata and creative assets (ad copy, titles, captions), destinatio...

[![Ticketmaster Scraper](https://img.shields.io/badge/Ticketmaster_Scraper-critical?style=for-the-badge)](https://apify.com/rigelbytes/ticketmaster-scraper)

A Ticketmaster-focused web scraper that extracts structured event metadata by location and date range for event monitoring, market research, and entertainmen...

[![Scrape Instagram Creators](https://img.shields.io/badge/Scrape_Instagram_Creators-informational?style=for-the-badge)](https://apify.com/rigelbytes/scrape-instagram-creators)

Scrape Instagram Creators is an Instagram profile and media scraper that extracts detailed creator profile metadata and media-level information. It captures ...

[![Immowelt Property Scraper](https://img.shields.io/badge/Immowelt_Property_Scraper-9cf?style=for-the-badge)](https://apify.com/rigelbytes/immowelt-property-scraper)

A scraper for immowelt.de (Germany) that harvests large volumes of real estate listings and returns structured property records for analysis. It extracts lis...

[![Immobilienscout24-scraper](https://img.shields.io/badge/Immobilienscout24_Scraper-blue?style=for-the-badge)](https://apify.com/rigelbytes/immobilienscout24-scraper)

A web scraping Actor that extracts large volumes of real estate listings and contact information from immobilienscout24.de, focused on German property market...

[![Instagram Creator Stats](https://img.shields.io/badge/Instagram_Creator_Stats-green?style=for-the-badge)](https://apify.com/rigelbytes/instagram-creator-stats)

A scraping and analytics Actor that extracts Instagram profile metadata and per-post media details to compute engagement metrics for creator/influencer analy...

[![Etsy Scraper](https://img.shields.io/badge/Etsy_Scraper-orange?style=for-the-badge)](https://apify.com/rigelbytes/etsy-scraper)

A web-scraping Actor that extracts structured product data from Etsy.com from category pages, search results, or individual product list URLs. It crawls list...

[![Rightmove Scraper](https://img.shields.io/badge/Rightmove_Scraper-blueviolet?style=for-the-badge)](https://apify.com/rigelbytes/rightmove-scraper)

Scrapes Rightmove.co.uk property listings and returns structured property records for real estate data extraction and analysis. The Actor crawls Rightmove se...

[![Outdoorsy Scraper](https://img.shields.io/badge/Outdoorsy_Scraper-red?style=for-the-badge)](https://apify.com/rigelbytes/outdoorsy-scraper)

A web scraping Actor that extracts rental listing data from outdoorsy.com search result pages. It processes multiple search result URLs in a single run, issu...

## Understanding Proxies:

When scraping data or browsing anonymously, proxies are essential. They act as intermediaries, masking your original IP address and allowing you to send requests from another location.

### Why Use Proxies?

- Avoid IP Blocks: By routing requests through proxies, you prevent the target website from recognizing your IP as a scraper or spammer.
- Access Geo-restricted Content: Proxies let you access content or websites restricted by location.
- Enhance Anonymity: Hide your actual IP, ensuring privacy while scraping or browsing.

### Types of Proxies

1. Residential Proxies

- Real IP addresses provided by ISPs to home users.
- They mimic regular users, making them harder to detect.
- Best for: Long-term, undetectable scraping, and avoiding blocks.
2. Data Center Proxies

- IP addresses from servers in data centers.
- Faster and cheaper than residential proxies but easier to detect and block.
- Best for: High-speed scraping, but with a higher risk of detection.
3. Mobile Proxies

- IPs provided by mobile carriers (3G/4G/5G networks).
- Very difficult to detect, as they appear as regular mobile users.
- Best for: Mobile-related scraping or avoiding sophisticated blocks.

### Rotating Proxies vs. Straight Proxies

- Rotating Proxies: Every request you send goes through a different proxy, making it harder for websites to detect patterns.
- Straight Proxies: All requests are sent through the same proxy, making it easier to track your IP.

## About Rigel Bytes

Rigel Bytes specializes in web scraping, automation, and data analytics. We help businesses extract and leverage valuable data for informed decision-making.

## Contact Us

Ready to unlock the power of data? Reach out to us at ([contact@rigelbytes.com](mailto:contact@rigelbytes.com)) or [book an appointment](https://cal.com/faizanali/appointments) with us to learn more about how we can help you achieve your data goals.

## Detailed Data

```
[
  {
    "pk": "18121785391719030",
    "user": {
      "is_verified": false,
      "id": "58456986501",
      "pk": "58456986501",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/658846606_17996342825946502_5111393810058833737_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=105&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=C3TOCepK-XAQ7kNvwFLUyxD&_nc_oc=Ado6r-XGlGMuIpdTpZkFbJzEEg9IEVBfK4PGh9Qb_irsxRmC5yO_gNsF1hKK-_Vv-Zk&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af2zxg4puiflxZCJYLjJUWfeG_oQ-0gJ7L-GwU_N6DdFWw&oe=69E66BBB",
      "username": "mc_gang04",
      "fbid_v2": "17841458395047123"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "😍",
    "giphy_media_info": null,
    "created_at": "2026-04-13T16:50:18",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "mc_gang04",
    "profile_link": "https://www.instagram.com/mc_gang04/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/658846606_17996342825946502_5111393810058833737_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=105&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=C3TOCepK-XAQ7kNvwFLUyxD&_nc_oc=Ado6r-XGlGMuIpdTpZkFbJzEEg9IEVBfK4PGh9Qb_irsxRmC5yO_gNsF1hKK-_Vv-Zk&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af2zxg4puiflxZCJYLjJUWfeG_oQ-0gJ7L-GwU_N6DdFWw&oe=69E66BBB"
  },
  {
    "pk": "18028046117804176",
    "user": {
      "is_verified": false,
      "id": "66431906102",
      "pk": "66431906102",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/485875878_587049927698512_5670905613732521566_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=109&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy43OTguQzMifQ%3D%3D&_nc_ohc=xdOX4fnJzJoQ7kNvwF-c2ZC&_nc_oc=AdqTfxm1DEGVZOwOvQhiH-_PdiJGiRe58ELEhdg9uO1xOBUNm1kp8AnwQv2bs9fF1MQ&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_ss=7a289&oh=00_Af1yahuTizng3Lfhs8jFmasGv21-BjQyrfIvAH_Mzt4cQA&oe=69E64E61",
      "username": "brandy_capello",
      "fbid_v2": "17841466303083988"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "😍😍",
    "giphy_media_info": null,
    "created_at": "2026-04-13T14:57:33",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "brandy_capello",
    "profile_link": "https://www.instagram.com/brandy_capello/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/485875878_587049927698512_5670905613732521566_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=109&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy43OTguQzMifQ%3D%3D&_nc_ohc=xdOX4fnJzJoQ7kNvwF-c2ZC&_nc_oc=AdqTfxm1DEGVZOwOvQhiH-_PdiJGiRe58ELEhdg9uO1xOBUNm1kp8AnwQv2bs9fF1MQ&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_ss=7a289&oh=00_Af1yahuTizng3Lfhs8jFmasGv21-BjQyrfIvAH_Mzt4cQA&oe=69E64E61"
  },
  {
    "pk": "18150493399463511",
    "user": {
      "is_verified": false,
      "id": "44276118053",
      "pk": "44276118053",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/619741112_18095448134478054_2218680027433513705_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=107&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=bWVCY5T8H9oQ7kNvwHvs1IY&_nc_oc=AdogSaME1YP92sZtPjLtBJdR0-dwMBStV7loTOS4WtNTf5wtERiTyV1jUva3hwVei9E&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af1U5RNYdDpnBKpXJpiun06pb0-V6nqkxNQxtENKmeCyag&oe=69E63D69",
      "username": "therealj0sh",
      "fbid_v2": "17841444341604514"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "",
    "giphy_media_info": {
      "first_party_cdn_proxied_images": {
        "fixed_height": {
          "url": "https://external.fsac1-2.fna.fbcdn.net/emg1/v/t13/2319285850170998249?stp=dst-src&url=https%3A%2F%2Fmedia2.giphy.com%2Fmedia%2Fv1.Y2lkPTA1NzQyMTNjcHR3ZmlsamZ2eTk1b2YwdTQ4dXN5MHF3NGt2YmZnbjlwcDlnazlpcyZlcD12MV9naWZzX2dpZklkJmN0PWc%2FaJ7Y5FRZHeHwQ%2F200.gif&utld=giphy.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_oc=AdqnLusKesnqYrUobkwDD2TZGMNifIqpNuYY8IXs_ZYID7fqTKmNgHX93E6scjWeRVA&ccb=13-1&oh=06_Q3--AaM6KD5VmHikcjS9onIMoWxBSinQ0dA_iGsIibjQnum8&oe=69E253A1&_nc_sid=1d65fc"
        }
      },
      "images": {
        "fixed_height": {
          "url": "https://static.cdninstagram.com/rsrc.php/v4/yr/r/xg_5YoVlvjp.gif"
        }
      },
      "id": "1690173535454984"
    },
    "created_at": "2026-04-13T13:13:33",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "therealj0sh",
    "profile_link": "https://www.instagram.com/therealj0sh/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/619741112_18095448134478054_2218680027433513705_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=107&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=bWVCY5T8H9oQ7kNvwHvs1IY&_nc_oc=AdogSaME1YP92sZtPjLtBJdR0-dwMBStV7loTOS4WtNTf5wtERiTyV1jUva3hwVei9E&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af1U5RNYdDpnBKpXJpiun06pb0-V6nqkxNQxtENKmeCyag&oe=69E63D69"
  },
  {
    "pk": "18199224088357408",
    "user": {
      "is_verified": false,
      "id": "55323705604",
      "pk": "55323705604",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/520664734_17983416029841605_8820000225135469917_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=108&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=T9JHL_tLYe4Q7kNvwG414qZ&_nc_oc=AdqJ341b5BoZyE98y28sgvapIcY-izIR6cDNrOPmnSr6ZhLuOPV9kTVJRFq4kA7tuKA&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af25KRoZDPI2vmdUlouk8AMR7IoCnV5c82PbT6roe6YrOg&oe=69E64643",
      "username": "luxevibe5only_",
      "fbid_v2": "17841455248135463"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "Follow me ❤️🔥",
    "giphy_media_info": null,
    "created_at": "2026-04-13T06:55:37",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "luxevibe5only_",
    "profile_link": "https://www.instagram.com/luxevibe5only_/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/520664734_17983416029841605_8820000225135469917_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=108&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=T9JHL_tLYe4Q7kNvwG414qZ&_nc_oc=AdqJ341b5BoZyE98y28sgvapIcY-izIR6cDNrOPmnSr6ZhLuOPV9kTVJRFq4kA7tuKA&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af25KRoZDPI2vmdUlouk8AMR7IoCnV5c82PbT6roe6YrOg&oe=69E64643"
  },
  {
    "pk": "17948263074072641",
    "user": {
      "is_verified": false,
      "id": "75121707823",
      "pk": "75121707823",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.75761-19/501197403_17842017711507824_3827231179005253638_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=103&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDI0LkMzIn0%3D&_nc_ohc=a5fcqHMv9jMQ7kNvwGeJxb-&_nc_oc=Adrzz-nslUHvGJ1ImRxKh2ZXQWVcEhuJOe_O8pcygclyof8_auLj2g8itmSyHdBgdYE&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af17D3hj__3WFI03t_loW6NNmCp7CBbqO8oOqOnE5L0Q_g&oe=69E64A12",
      "username": "cindy_liou8",
      "fbid_v2": "17841475234690213"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "哇！這個風格真的有點不一樣耶，好好奇接下來會有什麼驚喜～😍",
    "giphy_media_info": null,
    "created_at": "2026-04-13T03:10:14",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "cindy_liou8",
    "profile_link": "https://www.instagram.com/cindy_liou8/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.75761-19/501197403_17842017711507824_3827231179005253638_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=103&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDI0LkMzIn0%3D&_nc_ohc=a5fcqHMv9jMQ7kNvwGeJxb-&_nc_oc=Adrzz-nslUHvGJ1ImRxKh2ZXQWVcEhuJOe_O8pcygclyof8_auLj2g8itmSyHdBgdYE&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af17D3hj__3WFI03t_loW6NNmCp7CBbqO8oOqOnE5L0Q_g&oe=69E64A12"
  },
  {
    "pk": "18051175085742197",
    "user": {
      "is_verified": false,
      "id": "525769687",
      "pk": "525769687",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/422440444_933237154854351_2938189456321609024_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=106&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=Z5fIDjpujZAQ7kNvwEI5O5M&_nc_oc=Adr5fwqEKMHjuU0FHaQGjZNYK3_eJ4cSKqxwkFh-9s2rGYrK9ZaF7wdDMoH9l8Z2iN4&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_ss=7a289&oh=00_Af26efTVin8NkjFn3aZaWIhwo-7J8BVCKpIcNH5GYBV4oQ&oe=69E667F2",
      "username": "marypaulinepapas_",
      "fbid_v2": "17841400290618215"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "Actual Queen ❤️",
    "giphy_media_info": null,
    "created_at": "2026-04-13T02:02:05",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "marypaulinepapas_",
    "profile_link": "https://www.instagram.com/marypaulinepapas_/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/422440444_933237154854351_2938189456321609024_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=106&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=Z5fIDjpujZAQ7kNvwEI5O5M&_nc_oc=Adr5fwqEKMHjuU0FHaQGjZNYK3_eJ4cSKqxwkFh-9s2rGYrK9ZaF7wdDMoH9l8Z2iN4&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_ss=7a289&oh=00_Af26efTVin8NkjFn3aZaWIhwo-7J8BVCKpIcNH5GYBV4oQ&oe=69E667F2"
  },
  {
    "pk": "17854058193637224",
    "user": {
      "is_verified": false,
      "id": "71379150267",
      "pk": "71379150267",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/672403706_17909847657382268_2973406304777539636_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=109&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDc5LkMzIn0%3D&_nc_ohc=12-YuoZPVA4Q7kNvwG4e2y1&_nc_oc=AdrIgU99fXkMu9dSKcXrP-fAFsW83uMq1zQC8I5zt-80naVV0g4bQEvLyckAgdTiO3w&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af2iq9crsH_N8DLM6MeKSvoNKFjczcfc-2-3oRdnguDM-g&oe=69E6588E",
      "username": "zad_abdelreheem",
      "fbid_v2": "17841471468022393"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "❤️❤️❤️",
    "giphy_media_info": null,
    "created_at": "2026-04-12T23:53:03",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "zad_abdelreheem",
    "profile_link": "https://www.instagram.com/zad_abdelreheem/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/672403706_17909847657382268_2973406304777539636_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=109&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDc5LkMzIn0%3D&_nc_ohc=12-YuoZPVA4Q7kNvwG4e2y1&_nc_oc=AdrIgU99fXkMu9dSKcXrP-fAFsW83uMq1zQC8I5zt-80naVV0g4bQEvLyckAgdTiO3w&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af2iq9crsH_N8DLM6MeKSvoNKFjczcfc-2-3oRdnguDM-g&oe=69E6588E"
  },
  {
    "pk": "17963332398020023",
    "user": {
      "is_verified": true,
      "id": "80501115515",
      "pk": "80501115515",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/625749435_17845235595683516_843117470346257723_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=111&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy45NjAuQzMifQ%3D%3D&_nc_ohc=9yiPR8VT3GUQ7kNvwE58CrQ&_nc_oc=AdqI1tP7olUdiJ7HtseL0CKFltYirTd2rofgboiOnohlT-aUjJK34xndpBJYf07HlmU&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af0aeDOl3wPPsfc3FD2g7kxU4gB-r5NKCBM8IPxO6lhVTg&oe=69E6439F",
      "username": "hospital_pacman",
      "fbid_v2": "17841480505462639"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "Okay!",
    "giphy_media_info": null,
    "created_at": "2026-04-12T12:34:41",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "hospital_pacman",
    "profile_link": "https://www.instagram.com/hospital_pacman/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/625749435_17845235595683516_843117470346257723_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=111&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy45NjAuQzMifQ%3D%3D&_nc_ohc=9yiPR8VT3GUQ7kNvwE58CrQ&_nc_oc=AdqI1tP7olUdiJ7HtseL0CKFltYirTd2rofgboiOnohlT-aUjJK34xndpBJYf07HlmU&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af0aeDOl3wPPsfc3FD2g7kxU4gB-r5NKCBM8IPxO6lhVTg&oe=69E6439F"
  },
  {
    "pk": "17919551298325121",
    "user": {
      "is_verified": true,
      "id": "80501115515",
      "pk": "80501115515",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/625749435_17845235595683516_843117470346257723_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=111&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy45NjAuQzMifQ%3D%3D&_nc_ohc=9yiPR8VT3GUQ7kNvwE58CrQ&_nc_oc=AdqI1tP7olUdiJ7HtseL0CKFltYirTd2rofgboiOnohlT-aUjJK34xndpBJYf07HlmU&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af0aeDOl3wPPsfc3FD2g7kxU4gB-r5NKCBM8IPxO6lhVTg&oe=69E6439F",
      "username": "hospital_pacman",
      "fbid_v2": "17841480505462639"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "Ok",
    "giphy_media_info": null,
    "created_at": "2026-04-12T12:34:35",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "hospital_pacman",
    "profile_link": "https://www.instagram.com/hospital_pacman/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/625749435_17845235595683516_843117470346257723_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=111&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy45NjAuQzMifQ%3D%3D&_nc_ohc=9yiPR8VT3GUQ7kNvwE58CrQ&_nc_oc=AdqI1tP7olUdiJ7HtseL0CKFltYirTd2rofgboiOnohlT-aUjJK34xndpBJYf07HlmU&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af0aeDOl3wPPsfc3FD2g7kxU4gB-r5NKCBM8IPxO6lhVTg&oe=69E6439F"
  },
  {
    "pk": "17884293936526759",
    "user": {
      "is_verified": false,
      "id": "79594300725",
      "pk": "79594300725",
      "is_unpublished": false,
      "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/652640856_17855562825652726_6514904698387046877_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=107&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=QXk9nJ4kOmUQ7kNvwFif9cc&_nc_oc=AdpASPozTYbT7_fRhZ3RYLn82sMOxVOp02Cv4gbzueMMyCfEpp-9PL--gOLsIwXD4Hs&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af0wiRsPe8jqma_RsfGAXw8takSuTF8CWUrF2hUihV3jsw&oe=69E65CE1",
      "username": "glorionmedia",
      "fbid_v2": "17841479581769287"
    },
    "is_covered": false,
    "child_comment_count": null,
    "restricted_status": null,
    "has_translation": null,
    "has_liked_comment": false,
    "text": "Have you checked out The Money Signal podcast? The Einstein of Wall Street breaks down the week's biggest market stories in a way that actually makes sense 💡 Follow @moneysignal.podcast",
    "giphy_media_info": null,
    "created_at": "2026-04-12T09:54:29",
    "parent_comment_id": null,
    "comment_like_count": 0,
    "fallback_user_info": null,
    "__typename": "XDTCommentDict",
    "post_url": "https://www.instagram.com/p/DWte0fylh5b/",
    "username": "glorionmedia",
    "profile_link": "https://www.instagram.com/glorionmedia/",
    "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.82787-19/652640856_17855562825652726_6514904698387046877_n.jpg?stp=dst-jpg_s150x150_tt6&_nc_cat=107&ccb=7-5&_nc_sid=f7ccc5&efg=eyJ2ZW5jb2RlX3RhZyI6InByb2ZpbGVfcGljLnd3dy4xMDgwLkMzIn0%3D&_nc_ohc=QXk9nJ4kOmUQ7kNvwFif9cc&_nc_oc=AdpASPozTYbT7_fRhZ3RYLn82sMOxVOp02Cv4gbzueMMyCfEpp-9PL--gOLsIwXD4Hs&_nc_zt=24&_nc_ht=scontent.cdninstagram.com&_nc_gid=a_SHagTW88NVHoijrW8l5w&_nc_ss=7a289&oh=00_Af0wiRsPe8jqma_RsfGAXw8takSuTF8CWUrF2hUihV3jsw&oe=69E65CE1"
  }
]
```