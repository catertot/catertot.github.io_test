---
title: "Buttons"
description: "Click here!"
lead: "Click here!"
date: 2021-02-23 16:32:22
lastmod: 2021-02-23 16:32:27
draft: false
images: []
menu:
  docs:
    parent: "components"
weight: 100
toc: true
---

## Overview

### Solid

- Use solid buttons for primary actions on the page.
- Uses solid sol background to draw user's eye.
- Recommendation: Only use one primary action per major page section.

#### Live Example
{{< codepen id="fa4425d05fb8cf612144291a5d598a6b" >}}

### Secondary

Use secondary buttons for all actions that do not move the user to the next step or require additional user actions such as "Add to wish list" or "Find a campout near you."

[example here]

### Link Style

Do we want this? Idk

### Full Width

Displays at full width of its container.

[example here]

### Accessibility
Many WCAG requirements are contextual to their implementation. To ensure that usage of this component complies with accessibility guidelines you are responsible for the following:

- For icon-only buttons, provide `aria-label` text that describes the button's action
- If activating the button does not dismiss the current context, then focus typically remains on the button after activation, e.g., an Apply or Recalculate button.
- If a description of the button's function is present, the button element has `aria-describedby` set to the ID of the element containing the description.
- If the button is a toggle button, it has an `aria-pressed` state. When the button is toggled on, the value of this state is true, and when toggled off, the state is false.
- If the button action indicates a context change, such as move to next step in a wizard or add another search criteria, then it is often appropriate to move focus to the starting point for that action.
- Clearly and concisely describe the button's action or destination when the button is clicked or tapped:
  - For example, if the button text is "Shop now", the `aria-label` might read: "Shop our [specific advertising category] now"
- Avoid using "click here" or "start here" for buttons. If screen space for text is minimal:
  - Provide text that can be read by screen readers
- For buttons with the tag set to "`a`", always providing an `href` attribute. Empty `href` attributes are not considered true links

This component has no specific WCAG compliance attributes built into the control. It is possibile to define this component as a link or button:

- Select the semantically-correct element, which will ensure that assistive technologies have correct instructions for how to interact with the component
- Use the CdrLink component to make a button that looks like a link
- Do not use `div` or `input` elements
- Do not add `role="button"` to the CdrButton component
