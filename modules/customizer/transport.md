# Transport

 You can use the `transport` argument to define how your options will be applied to the preview.

 There are 3 choices available: `refresh`, `auto` and `postMessage`.

{% hint style="info" %}
**Read the `postMessage` docs too**

This argument uses the `postMessage` module. Please make sure you read the [documentation for the postMessage module](http://aristath.github.io/kirki/docs/modules/postmessage)
{% endhint %}

## refresh:

 By default all fields use the `refresh` method. This will force-refresh the preview pane in the customizer when the value changes.

## auto:

 If your field already contains an `output` argument you can set `transport` to `auto`. This will allow Kirki to auto-generate the `js_vars` argument according to your `output` and make the field work seamlessly both in the frontend and in the customizer without any code duplication.

## postMessage:

 If you use the `postMessage` method, you can either write your own Javascript to change things in the preview area or use the `js_vars` argument. If you decide to write your own scripts - which is highly advisable - we advise you to first read [this post on developer.wordpress.org](https://developer.wordpress.org/themes/advanced-topics/customizer-api/#using-postmessage-for-improved-setting-previewing) as well as this [blog post on Otto’s blog](http://ottopress.com/2012/how-to-leverage-the-theme-customizer-in-your-own-themes/).

