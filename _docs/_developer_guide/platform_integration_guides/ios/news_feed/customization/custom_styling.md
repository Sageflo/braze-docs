---
nav_title: Custom Styling
article_title: Custom News Feed Styling for iOS
platform: iOS
page_order: 0
description: "This reference article covers how to implement custom News Feed styling in your iOS application."
channel:
  - news feed

---

# Custom Styling

{% alert note %}
News Feed is being deprecated. Braze recommends that customers who use our News Feed tool move over to our Content Cards messaging channel—it's more flexible, customizable, and reliable. Check out the [migration guide]({{site.baseurl}}/user_guide/message_building_by_channel/content_cards/migrating_from_news_feed/) for more.
{% endalert %}

Integration of `SDWebImage` is required if you plan on using our Braze UI for displaying images within iOS in-app messages, News Feed, or Content Cards.

## Overriding default images

Braze allows clients to replace existing default images with their own custom images. To accomplish this, create a new `png` file with the custom image and add it to the app’s image bundle. Then, rename the file with the image’s name to override the default image in our library. Also, be sure to upload the `@2x` and `@3x` versions of the images to accommodate different phone sizes. Images available for override in Content Cards include: Images available for an override in the News Feed include:

* Read icon indicator: `Icons_Read`
* Placeholder image: `img-noimage-lrg`

{% alert important %} 
Overriding default images is currently not supported in our Xamarin iOS integration. 
{% endalert %}

