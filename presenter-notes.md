# Presenter notes

## 5. Wide range of disabilities

There are many different types of disabilities affecting people's abilities to touch, see, hear, or speak.

"Disabilities" could be permanent, temporary, or situational. For example, a parent may be holding a child while trying to use the phone; or a person may be in a noisy environment while trying to watch a video. People's normal abilities may be constrained by the situation, but they still need the same access to information.

## 6. Why is accessibility important?

In the US, the Department of Justice (DOJ) published the Americans with Disabilities Act (ADA) Standards for Accessible Design in September 2010. These standards state that all electronic and information technology must be accessible to people with disabilities.

Section 508 regulations are an amendment to the Rehabilitation Act of 1973 and apply to all information technology, including computer hardware, software and documentation. Section 508 requires federal agencies to make their information and communication technology accessible for everyone.

In addition to the law requirements, the web is originally designed for everyone. Everyone has abilities and limits to those abilities. Those limits should not be treated as obstacles to accessing the web.

Implementing accessibility can deepen our understanding of design. Considering things like tab order can take us beyond a vision of design as the look and feel and into the realm of user experience and usability. Accessibility is just another aspect of considering how to best build our sites to meet diverse human needs. The more we consider accessibility, the more profoundly we will understand user experience and anticipate user behavior—making us better designers.

## 8. WCAG

The Web Content Accessibility Guidelines (WCAG) is developed by the W3C. It is the international standard for making web content accessible. WCAG has been adopted by laws and standards in a lot of countries and regions. In the US, the Section 508 regulations incorporates WCAG 2.0.

## 9. WCAG 2.0 and 2.1

WCAG 2.0 was published in December 2008 and WCAG 2.1 was published in June 2018. WCAG 2.1 extends WCAG 2.0 by adding a number of new success criteria and guidelines.

Because WCAG 2.1 is relatively new and we are still learning the new guidelines. This webinar is based on the success criteria of WCAG 2.0.

## 10. Overview of WCAG 2.0

WCAG are organized by four basic principles:

1. Content must be **perceivable**.
2. Interface elements in the content must be **operable**.
3. Content and controls must be **understandable**.
4. Content must be **robust** enough to work with current and future technologies.

Each principle contains testable success criteria, which are set at three levels: A, AA, and AAA.

## 11. What we will cover today

So we have selected a few topics that are probably the most fundamental accessibility requirements for any web pages: keyboard focus, tab order, color and color contrast, and text alternatives. These are great foundations to start learning about accessibility. They are easy to relate to and test, and they benefit virtually all users.

For each topic, we will discuss relevant WCAG success criteria and then we will show you a few examples of how to meet those success criteria.

One question we get a lot is how to make maps accessible, particularly for non-sighted users. In this webinar we will show our initial attempt at addressing this challenge. And we certainly welcome any input or feedback from you.

Finally, we will talk about a do-it-yourself process for testing accessibility. Working to accommodate a diverse range of abilities means there are a correspondingly diverse range of issues to consider. We break down these issues into a logical, step by step process so that we all can follow.

## 12. Our focus today

We understand that accessibility can be a complex and difficult topic. So in this webinar, we will be focusing on the fundamental topics of accessibility, how to get started, and how we can take simple actions to identify accessibility issues.

## 13. Past presentations

We will try not to dive deep into the code for this webinar. If you are a developer who is interested in more technical discussions, we gave two presentations about web accessibility at last year's Esri Developer Summit. We have included links to the recordings on this slide.

## 14. Presentations at DevSummit 2019

In addition to today's webinar, there will be three presentations on web accessibility at this year's Developer Summit. I have listed the links and times on this slide. Even though the titles are the same, we will prepare new content for the presentations. So if you are planning to attend the Developer Summit this year, we hope to see you at these presentations.

## 15. Focus and tab order

### WCAG 2.4.7 Clear focus

Focus is the visual indicator that shows which control on the screen currently receives input from the keyboard. If users use keyboard to navigate a page, they should be able to see which control they are on at any time.

The best way to ensure clear focus is to have a visible border or outline around the element in use, whether it’s a form field, link, menu, content area or any other interactive element. This makes it easier for your users to understand where they are on a page.

Browsers have default styles for focus. We could customize the focus style if needed, but don't just disable the browser's default focus style.

### WCAG 1.3.2 Tab order

Tab order is the order in which focus proceeds forward and backward through interactive elements via the Tab key. As a keyboard user navigates through the page, the order in which interactive items receive keyboard focus is important.

The default keyboard navigation order must be logical and intuitive. For example, in English we read from left to right and from top to bottom. So the tab order should follow the visual flow of the page: left to right and top to bottom. And we should let the web page's source code determine the tab order.

I should point out that letting the keyboard focus jumping around on the page is not only an accessibility issue, but also a usability issue. It just makes using the keyboard to work with the page a lot harder than necessary.

### WCAG 2.1.1 Keyboard access

Many people use keyboard to use a web page. Some of them may have motor impairment, and some may be power users that are faster with keyboard. Like mouse users, keyboard users should be able to use forms, menus, or any other functionalities on a web page.

### WCAG 2.1.2 Keyboard trap

A keyboard trap occurs when a user can get into a subsection on a web page by using the keyboard, but the user cannot get out of that subsection through the keyboard.

A common exception of this rule is when we show a modal dialog to the user, the dialog needs to trap keyboard focus until the user chooses to close the dialog. This is because the dialog introduces a new workflow to the user and needs the user's input to complete the new workflow.

## 20. Color and color contrast

### WCAG 1.4.1 Color only info

Users with visual impairment need help when we use color on the web. As many as 1 in 12 men have some degree of color blindness. That means about 8% of male users may struggle if we don't use color correctly. For example, if we use red text only to show an error message, users who cannot see red will not notice that message is an error. So that error message needs at least one more means to convey the meaning, like an error icon.

As another example, when we use color only to show different datasets in a chart, color blind users may not understand the different datasets. We should add clear labelling and patterns to those datasets, in addition to colors.

This guideline is not about removing color from our web pages or making web pages black and white, far from it. It just means that color should not be the only way of conveying information. Adding additional ways of conveying the same information in a lot of cases not only improves the accessibility, but also the overall user experience.

### WCAG 1.4.3 Contrast ratio

All of us will benefit from a good contrast between text and its background color. For users with visual impairments, good contrast is essential.

## 22. White text on colored background

When using white text on a colored background, it is sometimes hard to achieve a good contrast. You may be surprised how dark the color needs to be to meet the 4.5 contrast ratio. This can create hierarchy issues when those elements are not supposed to be the focus of the page - dark colored backgrounds will really grab the user's attention.

## 23. Flipping the contrast

You can solve the problem by flipping the contrast. Instead of using light text on a dark colored background, use dark colored text on a light colored background. The color is still there to help support the text, but it's way less prominent and does not interfere as much with other parts of the page.

## 25. Text alternatives

### WCAG 1.1.1 Text alternatives

Alternative (or 'alt') text is a text replacement for non-text content like images. Non-sighted users rely on the alternative text to understand information in images. When they use screen reader and encounter an image, the screen reader will announce the alt text of the image. If the image does not have alt text, the screen reader will usually announce the file name of the image, which is not useful.

A common exception for this guideline is that if an image is decorative and it does not convey meaning, we should set the alternative text to an empty string.

## 28. Accessible maps
There are several options for making map content accessible. If the map is a simple map showing a location or providing directions you can provide a text description of the map. Here’s an example where the map image shows the location of the Esri Olympia regional office with a text description below the map.

If the map is more complicated and shows several features you can provide the information in an alternate format such as a text list of locations or a table.

## 29. Default map navigation

The 2D Map View and 3D Scene View available in the Esri JavaScript api both provide out of the box support for navigating the map via the keyboard. Check out the documentation at <a href="https://developers.arcgis.com/javascript"/>https://developers.arcgis.com/javacript</a> for details.

## 32. DIY accessibility test

So we recommend a four-step process to test accessibility of web applications. The four steps are automated test, keyboard test, screen reader test, and color test.

This is also the process we follow at Esri. It breaks down the testing to a logic flow, and it minimizes the switching between different types of tests that we need to do.

## 33. Automated test with aXe

aXe is an extension that you can install in Chrome and Firefox. It tests the rendered page in Chrome and Firefox. It reports any violations against a set of accessibility rules and best practices. A big advantage of aXe, compared to other automated testing tools, is that it is relatively conservative, meaning it tends to report less false positives. And aXe itself is accessible. Keyboard users and non-sighted users should be able to use aXe for automated tests.

(After demo:) I should point out that automated tests cannot replace manual tests using keyboard and screen reader. Automated test tools like aXe can help us quickly find certain types of issues, but not all. For example, an automated test tool can tell us an image is missing alt text, but it cannot judge whether an alt text is meaningful for the image.

## 35. Keyboard test

The second step is keyboard test. This means using the Tab key or Shift and Tab keys to move focus on the page, using Enter key to click links, and using Enter or Space key to click buttons. Some interactive elements, like menus, tabs, or select, may require the arrow keys.

The goal of the keyboard test is to see if the web page provides the same functionalities to keyboard users as mouse users. It may help to unplug or disable the mouse, and try to use the keyboard to perform the tasks that mouse users would do. If an interactive element does not have keyboard focus or it cannot be tabbed to, there is a keyboard accessibility issue. If the focus jumps around on the page, there could be a keyboard accessibility issue as well.

## 36. Screen reader

The third step is testing using screen readers.

A "screen reader" is the generic term for a program that helps blind people use a computer. Simply put, a screen reader will "read" (speak) the content of a page to the blind user.

A blind person using a screen reader experiences a website linearly, a little bit at a time. If an element does not have enough information for the screen reader to read what it is, the blind user may have difficulty understanding what the element is meant for.

Due to time limitation, we will not discuss details of using screen readers. But here is recommended pairing between screen readers and browsers. VoiceOver is the built-in screen reader in MacOS, so it works well with Safari. NVDA is a free screen reader in Windows and it is recommended for Firefox. Jaws is another screen reader in Windows and traditionally it works well with Microsoft browsers like IE and Edge. Jaws requires a paid license.

## 37. Screen reader basics

We recommend these two video tutorials for VoiceOver and NVDA. They cover the basic commands to read and interact with web content for testing purposes. Both of the videos are parts of the a11ycasts series on Youtube. We will share this presentation so you will have the URLs.

## 38. Color test

The last step is manual color test. This step is necessary because automated test tools cannot cover all color issues. For example, a background may use color gradient, not a single color. And for information like error messages, we have to manually look at it to see if they use color only to communicate the meaning.

## Last

That concludes our presentation. We will now move over to Amy for questions.
