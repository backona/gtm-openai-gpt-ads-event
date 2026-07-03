# OpenAI ChatGPT Ads Event GTM Tag Template by [Backona](https://backona.com)

Google Tag Manager template to send [OpenAI Ads Measurement Pixel](https://developers.openai.com/ads/measurement-pixel) (`oaiq`) conversion events for ChatGPT ad attribution. Built by [Backona](https://backona.com).

Requires the separate **OpenAI ChatGPT Ads Configuration** template to load `oaiq` first ([gtm-openai-gpt-ads-config](https://github.com/backona/gtm-openai-gpt-ads-config)).

Release history: [CHANGELOG.md](./CHANGELOG.md).

This repository publishes **OpenAI ChatGPT Ads Event** ([gtm-openai-gpt-ads-event](https://github.com/backona/gtm-openai-gpt-ads-event)).

| Template | Purpose |
|----------|---------|
| [**OpenAI ChatGPT Ads Event**](https://github.com/backona/gtm-openai-gpt-ads-event) | Send `oaiq('measure', …)` conversion events |
| [OpenAI ChatGPT Ads Configuration](https://github.com/backona/gtm-openai-gpt-ads-config) | Load SDK and run `oaiq('init', …)` |

## Install

1. Install **OpenAI ChatGPT Ads Configuration** from the [Community Template Gallery](https://tagmanager.google.com/gallery) or [gtm-openai-gpt-ads-config](https://github.com/backona/gtm-openai-gpt-ads-config). Set its trigger to **Initialization - All Pages**.
2. Add **OpenAI ChatGPT Ads Event** from the [Community Template Gallery](https://tagmanager.google.com/gallery) or [gtm-openai-gpt-ads-event](https://github.com/backona/gtm-openai-gpt-ads-event), or import [`template.tpl`](./template.tpl) from this repository.
3. Create a tag using **OpenAI ChatGPT Ads Event**.
4. Choose a standard event (or **Custom**) and fill in optional value, plan, and event contents as needed.
5. Set a conversion trigger (purchase, form submit, page view, etc.).

Supported JavaScript Pixel events: `page_viewed`, `contents_viewed`, `items_added`, `checkout_started`, `order_created`, `lead_created`, `registration_completed`, `appointment_scheduled`, `subscription_created`, `trial_started`, and custom events. See [send events](https://developers.openai.com/ads/measurement-pixel#send-events).

`app_installed` and `app_opened` are not supported by the JavaScript Pixel - use the Conversions API server-side.

## Consent

On each tag, open **Advanced settings → Consent settings** and consider these types when using [Consent Mode v2](https://support.google.com/tagmanager/answer/10718549):

- `ad_storage`
- `ad_user_data`
- `ad_personalization`
- `analytics_storage`

For consent banners and defaults, see [Backona Cookie Consent Management](https://backona.com/product/cookie-consent-management).

## Support

Report bugs or request features via [GitHub Issues](https://github.com/backona/gtm-openai-gpt-ads-event/issues) on this repository.
