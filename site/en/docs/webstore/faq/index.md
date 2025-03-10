---
layout: "layouts/doc-post.njk"
title: Frequently Asked Questions
date: 2020-06-09
updated: 2021-07-27
description: Frequently asked questions about Chrome Web Store.
---

The [Chrome Web Store][1] lets you publish free or paid extensions where Google Chrome users can easily
find them. This FAQ answers many common questions about the Chrome Web Store. If you don't find your
answer here, check the [extension hosting changes FAQs][2], the [general extension FAQs][3], or the
[chromium-apps group][4].

Please expand the _Table of Contents_ to quickly navigate this page.

## General Questions

### What is the Chrome Web Store? {: #faq-gen-01 }

The Chrome Web Store is an open marketplace for [Google Chrome
Extensions][ext] and [Google Chrome Themes][themes], where consumers may browse, install, and
purchase items and install them in their browser. These items are built with web technologies and
run inside of web browsers.

### How many people use Chrome? {: #faq-gen-02 }

In 2015, Google announced one billion active users for Chrome. It's also important to note that
Chrome Web Store extensions can run in any browser that supports the web technologies used to build the
extension.

### Is there a road map for Chrome? {: #faq-gen-05 }

You can follow the [Google Chrome Releases blog][95] to learn about all the latest changes that are
being made to Chrome. You can create and track bugs and features in the [Chromium bug tracker][96],
and we recommend that you download and install the [Dev channel build][97] of Chrome browser.

### Why would someone install an extension instead of just using a bookmark or typing in a URL? {: #faq-gen-07 }

Installing an extension ensures it is launchable from the New Tab Page via the Chrome extensions launcher.
Installing an extension also allows you to grant it privileges such as unlimited local storage and
background pages.

### Is there an approval process for extensions in the store? {: #faq-gen-08 }

All extensions go through an automated review process and in some cases, an extension will be published without
further manual review. There may be some instances in which a manual review will be required before
the extension is published based on our [program policies][98]. In some cases, where sensitive permissions
are requested, review times and/or approval times may be longer.

### How will users find my extension? {: #faq-gen-09 }

The Chrome Web Store will surface extensions in a variety of ways. Of course, each extension gets a page in
the store, which will be searchable via the store and other search engines. There will be category
lists in the store, as well as a variety of curated and algorithmically generated lists. We
recommend that you broadly promote your extension, through marketing websites and other means, so that
users will find your extension even outside of the store.

### Why am I being asked to pay a registration fee? {: #faq-gen-11 }

The registration fee helps to prevent fraud in the Chrome Web Store. You need to pay this one-time
fee before you can access the Chrome Web Store Developer Dashboard.

{% Aside %}
If you are already using the developer dashboard but haven't paid this fee yet, you must
now pay it in order to continue accessing your developer dashboard. This one-time fee is now part of
the standard [developer registration process][99].
{% endAside %}

### What types of extensions are not allowed in the store? {: #faq-gen-22 }

While we try to allow most extensions, a small number of extensions are explicitly
disallowed in our [Developer Terms of Service][102] and [Program Policies][103]. Such
extensions will be removed when they are brought to our attention.

### How do I report an abusive extension? {: #faq-gen-23 }

To report an extension which violates our Terms of Service, locate the corresponding listing
in the store and use the "Report abuse" link.

### How are items ranked in the store? {: #faq-gen-24 }

Items in the store are ranked or featured in order to make it easier for users to find high quality
content. Ranking is performed by a heuristic that takes into account ratings from users as well as
usage statistics, such as the number of downloads vs. uninstalls over time.

Other factors include the following:

- The design is pleasant to the eye.
- The item provides a clear purpose and fills a real user need.
- The setup and onboarding flow are intuitive.
- The item is easy to use.

### What are "By Google" extensions?

Certain extensions on the Chrome Web Store are marked as "By Google". These extensions have been
developed by Google and go through a rigorous review process. You may also search specifically for
these extensions by checking the "By Google" checkbox on the search pages.

### How are "Featured" items selected? {: #faq-gen-25 }

The Chrome Web Store team occasionally selects interesting listings as "Featured" listings. We're
not accepting requests to be featured at this point, since that would quickly become unmanageable.
Here are a few tips to increase the likelihood that we'll feature your listing:

- Write a great piece of software
- Make sure your listing looks really nice (nice icon, good descriptions, crisp screenshots and/or
  videos)
- Promote your listing independently so that it starts to rise in the rankings

### How can my extension be selected for a collection? {: #faq-gen-26 }

The collections are curated, and are not intended to be comprehensive. A collection is curated using
the ranking criteria already listed and may be selected to provide helpful results for certain
circumstantial situations, such as work-from-home extensions. Solicitations to be placed in a
collection are not accepted.

### How can I provide support for users of my extension? {: #faq-gen-27 }

You can set up discussion groups to communicate with your users. One way of doing so is through
[Google Groups][104].

### Can I remove comments from my listing if I believe they are unfair? {: #faq-gen-28 }

No, you can't remove user comments. However, we encourage you to respond to user feedback in the
comments to show that you are addressing their concerns.

You may also report fake reviews via the Developer [Support Form][cws-support].

### Is there a limit to the number of items I can have on the Chrome Web Store? {: #faq-gen-29 }

You can upload as many items to the Chrome Web Store as you like, but by default, you are limited to
having a total of 20 published items at any one time. This limit applies to the sum of your Chrome
Apps and Chrome Extensions as a total—it is not 20 of each item. If you reach this limit, [you may
request a limit increase][cws-support]. The Chrome Web Store staff will review your existing items and your
developer account history, and if approved, you will be granted an increase. Please note that if
your developer account has been suspended in the past, or you have had items taken down previously
for policy violations, or your items consistently receive low quality ratings, your request may be
denied.

### Can I obfuscate my code? {: #faq-gen-30 }

As of October 1st 2018, developers must not obfuscate code or conceal functionality of their
extensions. This also applies to any external code or resource fetched by the extension package. For
more information, please review our [program policies][106].

## Development

### How do I write an extension? {: #faq-dev-01 }

You can find all the information you need to develop extensions at [/docs/extensions/][ext].

### How can I push an update of my code to my users? {: #faq-dev-02 }

Visit [https://chrome.google.com/webstore/devconsole][110] and click on the listing you wish to
update. Once you upload a new version and click **Publish**, your update will automatically be
pushed out to users over the next few hours.

### Can I host my own extension? {: #faq-dev-03 }

Yes, you may host your own extension, although you will need to take care of [packaging and
serving][111] the [auto-update manifest][112] yourself.

## Creating a listing

### In what format should I upload my code? {: #faq-listing-01 }

To upload an item to the Chrome Web Store, submit a ZIP file containing the files used in your
extension. Do not upload a .crx file; the submission will fail.

### How long will it take for my listing to appear in the store? {: #faq-listing-02 }

The item won't appear in the web store until it has successfully completed the review process.
(Although the item's unique ID is generated as soon as you upload your first zip file.) For further
details, see [How long will it take to review my item?][114].

Extensions which are published to the same domain as the publisher address may be approved more
quickly.

### How can I remove my listing from the store? {: #faq-listing-03 }

Visit the [developer dashboard][dev-dashboard]. Click the item you want to
remove from the store, so that the edit page for that item appears. Then click the "more options"
icon in the top right-hand corner and select **Unpublish**. Your listing will no longer be visible
in the store.

{% Img src="image/BhuKGJaIeLNPW9ehns59NfwqKxF2/GdnJe3SsuL84LFkLODZl.png", alt="Screenshot of how to unpublish an item", width="299", height="205" %}

### What are the screenshot and text requirements for the store? {: #faq-listing-04 }

See [Supplying Images][116] for guidelines on supplying images for the store. Some other best
practices to consider:

- Write a catchy title, a clear and descriptive short description, and a detailed long description.
- Create screenshots that demonstrate how your extension works.
- Upload a screencast, such as a YouTube video or a Google Docs Presentation, to demonstrate how
  your extension works.
- Post a support link so that users don't clutter your comments thread with bug reports.

### How can I import an existing extension into the store? {: #faq-listing-05 }

You may import an extension with a pre-existing key into the store (see [instructions][117]).

### How can I export an extension from the store? {: #faq-listing-06 }

Currently we do not support exporting a listing's sources or private key from the store.

### Why did I receive a "Cannot parse the manifest" error when uploading my extension? {: #faq-listing-07 }

The manifest file needs to be in JSON format. Most likely, you've included a comment in the manifest
file that is not recognized by the Chrome Web Store's JSON parser. Try removing any comments from
the manifest file and try re-uploading.

### I've verified my domain, and I have a wildcard URL like \*://example.com, but the Chrome Web Store is still asking me to verify my domain. What gives? {: #faq-gen-15 }

If you use a wildcard like \*://example.com, make sure you have verified both http://example.com and
https://example.com.

### When I try to upload to the Chrome Web Store, I get this error: "(Server rejected) An error occurred: please try again later." What gives? {: #faq-gen-16 }

This error occasionally occurs if you've been logged into the Chrome Web Store for a long time. If
you sign out of your Google Account and then sign back in, you should be able to upload your
extension.

### Can I control the regions where my extension is listed? {: #faq-gen-18 }

Yes, you can select which regions your extension appears in. This might be because your extension is
only applicable to the local market, or you might have specific obligations that mean you can only
make your extension available in certain regions.

### How do I localize my listing in the store? {: #faq-gen-19 }

There are two points where you need to localize your extension for listing in a region that isn't your
home market.

1.  Your extension package. See [Internationalizing Your App][internationalize] for information on localizing your
    extension's presence inside Chrome.
2.  Your detailed listing. The developer dashboard now includes the ability for you to select all
    the regions that you want your application to appear in, allows you to localize the detailed
    description, price points relative to the market you are in, and screenshots.

### How do I localize my detailed description? {: #faq-gen-20 }

You first need to [internationalize][internationalize] your extension and specify a "default_locale" attribute in your
manifest. Once you upload your internationalized extension, a selection box will appear at the top of your
extension listing, allowing you to switch between languages that you support and change the detailed
description.

### How do I show different screenshot images per region? {: #faq-gen-21 }

Visit your extension page in the [Chrome Web Store Developer Dashboard][dev-dashboard], change the currently
selected language to your desired choice (for example "en-GB") and upload a screenshot as normal.
Once the image is uploaded you will be presented with an option to "Show this item in **all**
locales" or "Show this item **only** in the 'en-GB' locale". Select the later to show the screenshot
to only users of the "en-GB" Chrome Web Store.

### My item's status says "pending review." What does this mean? {: #faq-listing-08 }

This means that you've submitted your item for publishing and it is currently in the queue to be
reviewed. The item will not appear in the store until it passes this review. (See also [How long
will it take to review my item?][121])

### How long will it take to review my item? {: #faq-listing-108 }

Review times vary; some reviews complete in a few hours, others take many days, and in some cases a
review can take several weeks. Some reasons that an item could require more extensive review
include:

- The item is suspected to contain or to be distributed by malware or unwanted software.
- The item is suspected to violate one of the developer program policies.
- The item may have already been previously removed for a legal or policy violation, and has been
  resubmitted.
- The item requests powerful permissions that require in-depth review.

Note that all item submissions—whether for a new item or an update to an existing one—are
subject to the same review process.

For more information about the unwanted software policy, see:
[https://www.google.com/about/company/unwanted-software-policy.html][122].

For more information about the developer program policies, see:
[/webstore/program_policies][123].

If your item's status says "pending review" for more than three weeks, you should [contact
support][cws-support].

### Why isn't my extension showing up on search? {: #faq-listing-09 }

It depends. There are several reasons why your item may not be showing up in search.

- You just published your extension. It might take a few hours before we index it.
- Your extension manifest is out of date. Upgrade your item to a current valid manifest version as
  described [here][125].
- Your extension is not listed in the region you are searching in. See more details [here][127].

### My extension has been removed from the Chrome Web Store. What should I do? {: #faq-listing-10 }

Application removals count as strikes against the good standing of your developer account. Multiple
or egregious policy violations may result in termination of your developer account.

- For all policy violation extension removals, you will receive a removal notification email with more
  details in the developer account listed as the owner of the extension. Please make the appropriate
  changes so your extension complies with all [Developer Program Policies][128], [Branding
  Guidelines][129] and [Terms of Services][130]. Once you have remedied the violation you can
  resubmit via your developer dashboard.
- Please do not re-publish a removed extension until the policy violation has been remedied. If
  you have additional questions or feel your item was wrongly removed, you can reply directly to the
  removal email and appeal.
- If you believe your developer account was wrongly terminated, you can appeal [here][cws-support]. We will
  only reinstate accounts if an error was made, and a re-review finds that your account does not
  violate the developer terms.

### How do I link my Play and Chrome Web Store item so that the "Available for Android" link appears on my item detail page? {: #faq-listing-11 }

We regularly run a script that looks for exact matches between the item name and the developer email
address in Play and CWS. If there is an exact match, the "Available for Android" link will
automatically show up on your item detail page the next time the script runs. At this point, there
is no way to enter the information into your listing.

## Additional Troubleshooting

If you've fixed all errors produced by the tools and continue experiencing issues, please [contact
us][cws-support] with any additional details regarding the problem. Please send us a screenshot of the
problem and include your .crx file.

### How can I raise P2B concerns?

European developers can raise concerns about clarity of terms, policies, or other Platform To
Business related issues by contacting CWS support.

[1]: https://chrome.google.com/webstore
[2]: /docs/extensions/mv2/hosting_changes
[3]: /docs/extensions/mv2/faq
[4]: https://groups.google.com/a/chromium.org/group/chromium-apps
[5]: #faq-gen-01
[6]: #faq-gen-02
[7]: #faq-gen-05
[8]: #faq-gen-06
[9]: #faq-gen-07
[10]: #faq-gen-08
[11]: #faq-gen-09
[12]: #faq-gen-11
[13]: #faq-gen-17
[14]: #faq-gen-22
[15]: #faq-gen-23
[16]: #faq-gen-24
[17]: #faq-gen-25
[18]: #faq-gen-26
[19]: #faq-gen-27
[20]: #faq-gen-28
[21]: #faq-gen-29
[22]: #faq-gen-30
[23]: #faq-dev-01
[24]: #faq-gen-10
[25]: #faq-dev-02
[26]: #faq-dev-03
[27]: #faq-listing-01
[28]: #faq-listing-02
[29]: #faq-listing-03
[30]: #faq-listing-04
[31]: #faq-listing-05
[32]: #faq-listing-06
[33]: #faq-listing-07
[34]: #faq-gen-15
[35]: #faq-gen-16
[36]: #faq-gen-18
[37]: #faq-gen-19
[38]: #faq-gen-20
[39]: #faq-gen-21
[40]: #faq-listing-08
[41]: #faq-listing-108
[42]: #faq-listing-09
[43]: #faq-listing-10
[44]: #faq-listing-11
[45]: #faq-payments-01
[46]: #faq-payments-02
[47]: #faq-payments-03
[48]: #faq-payments-04
[49]: #faq-payments-05
[50]: #faq-payments-06
[51]: #faq-payments-07
[52]: #faq-payments-09
[53]: #faq-payments-10
[54]: #faq-payments-11
[55]: #faq-payments-12
[56]: #faq-payments-13
[57]: #faq-payments-14
[58]: #faq-payments-15
[59]: #faq-payments-16
[60]: #faq-app-01
[61]: #faq-app-02
[62]: #faq-app-02.5
[63]: #faq-app-03
[64]: #faq-app-04
[65]: #faq-app-05
[66]: #faq-app-06
[67]: #faq-app-07
[68]: #faq-app-08
[69]: #faq-app-09
[70]: #faq-app-10
[71]: #faq-app-11
[72]: #faq-app-12
[73]: #faq-app-13
[74]: #faq-app-14
[75]: #faq-app-15
[76]: #faq-app-16
[77]: #faq-app-17
[78]: #faq-app-18
[79]: #faq-app-19
[80]: #faq-app-20
[81]: #faq-app-21
[82]: #faq-app-22
[83]: #faq-app-23
[84]: #faq-app-24
[85]: #faq-app-25
[86]: #faq-app-26
[87]: #faq-app-27
[88]: #faq-extensions-01
[89]: #faq-extensions-02
[90]: #faq-themes-01
[91]: #faq-themes-02
[95]: https://chromereleases.googleblog.com/
[96]: https://crbug.com
[97]: https://www.chromium.org/getting-involved/dev-channel
[98]: /docs/webstore/program_policies
[99]: /docs/webstore/register
[100]: https://www.google.com/accounts/NewAccount
[102]: /docs/webstore/terms
[103]: /docs/webstore/intl/en/program_policies.html
[104]: https://groups.google.com
[106]: /docs/webstore/program_policies
[110]: https://chrome.google.com/webstore/devconsole
[111]: https://code.google.com/chrome/extensions/packaging.html
[112]: https://code.google.com/chrome/extensions/autoupdate.html
[114]: #faq-listing-108
[116]: images
[117]: https://groups.google.com/group/chromium-extensions/browse_thread/thread/defbf282d11a8cc4/a2d1aedb84bc60b9
[121]: #faq-listing-108
[122]: https://www.google.com/about/company/unwanted-software-policy.html
[123]: /docs/webstore/program_policies

[125]: /docs/extensions/mv3/manifestVersion
[127]: https://support.google.com/chrome_webstore/answer/1254182?hl=en&ref_topic=1734051
[128]: /docs/webstore/program_policies
[129]: /docs/webstore/branding
[130]: /docs/webstore/terms

[apps]: /docs/apps/
[cws-support]: https://support.google.com/chrome_webstore/contact/developer_support/
[ext]: /docs/extensions/
[dev-dashboard]: https://chrome.google.com/webstore/developer/dashboard
[internationalize]: /docs/webstore/i18n
[themes]: /docs/extensions/mv3/themes/

