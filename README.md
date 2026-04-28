# Getting Started Guide: PayPal Buy Button example

Try it out now in GitHub Codespaces... [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/paypaldev-community/getting-started-guide-buy-button)

## Preview

![PayPal Buy Button example](assets/preview.png)

## Explaination

### Step 1

In your html `<head>` tag add the following: (this has your unique `client-id`).

```html
<script src="https://www.paypal.com/sdk/js?client-id=BAAY5EAkskLsBGeYrYpHm9PzA-KkgOiOx1J0fwKCo_YkS3f81HiV-Ze9QzwmGHyf4S2cZjRtpTRc6pDekA&components=hosted-buttons&disable-funding=venmo&currency=USD"></script>
```

> [!IMPORTANT]
> This should be included only once per page.

### Step 2

In your html `<body>` tag add the following:

```html
<div id="paypal-container-ZGT7S2VPTE4D4"></div>
<script>
  paypal
    .HostedButtons({
      hostedButtonId: "ZGT7S2VPTE4D4",
    })
    .render("#paypal-container-ZGT7S2VPTE4D4");
</script>
```

> [!TIP]
> You can create as many buttons as you need for different products or services. Just make sure to use the specific hostedButtonId for each button you create, which you can find in your PayPal dashboard under the details of each button you create.

## How to create your PayPal Buy Button

![Demo on how to create your PayPal Buy Button](assets/paypal-create-button.gif)
