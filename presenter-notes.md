# Presenter notes

## 3. Wide range of disabilities

There are many different types of disabilities affecting people's abilities to touch, see, hear, or speak.

"Disabilities" could be permanent, temporary, or situational. For example, a parent may be holding a child while trying to use the phone; or a person may be in a noisy environment while trying to watch a video. People's normal abilities may be constrained by the situation, but they still need the same access to information.

## 4. Why is accessibility important?

In the US, the Department of Justice (DOJ) published the Americans with Disabilities Act (ADA) Standards for Accessible Design in September 2010. These standards state that all electronic and information technology must be accessible to people with disabilities.

Section 508 regulations are an amendment to the Rehabilitation Act of 1973 and apply to all information technology, including computer hardware, software and documentation. Section 508 requires federal agencies to make their information and communication technology accessible for everyone.

In addition to the law requirements, the web is originally designed for everyone. Everyone has abilities and limits to those abilities. Those limits should not be treated as obstacles to accessing the web.

Implementing accessibility can deepen our understanding of design. Considering things like tab order can take us beyond a vision of design as the look and feel and into the realm of user experience and usability. Accessibility is just another aspect of considering how to best build our sites to meet diverse human needs. The more we consider accessibility, the more profoundly we will understand user experience and anticipate user behavior—making us better designers.

## 6. WCAG

The Web Content Accessibility Guidelines (WCAG) is developed by the W3C. It is the international standard for making web content accessible. WCAG has been adopted by laws and standards in a lot of countries and regions. In the US, the Section 508 regulations incorporates WCAG 2.0.

## 7. WCAG 2.0 and 2.1

WCAG 2.0 was published in December 2008 and WCAG 2.1 was published in June 2018. WCAG 2.1 extends WCAG 2.0 by adding a number of new success criteria and guidelines.

Because WCAG 2.1 is relatively new and we are still learning the new guidelines. This webinar is based on the success criteria of WCAG 2.0.

## 8. Overview of WCAG 2.0

WCAG are organized by four basic principles:

1. Content must be **perceivable**.
2. Interface elements in the content must be **operable**.
3. Content and controls must be **understandable**.
4. Content must be **robust** enough to work with current and future technologies.

Each principle contains testable success criteria, which are set at three levels: A, AA, and AAA.

## 9. What we will cover today

So we have selected a few topics that are probably the basic accessibility requirements for any web pages: keyboard focus, tab order, color and color contrast, and text alternatives. These are great foundations to start learning about accessibility. They are easy to relate to and test, and they benefit virtually all users.

One question we get a lot is how to make maps accessible, particularly for non-sighted users. In this webinar we will show our initial attempt at addressing this challenge. And we certainly welcome any input or feedback from you.

Finally, we will talk about a do-it-yourself process for testing accessibility. Working to accommodate a diverse range of abilities means there are a correspondingly diverse range of issues to consider. We break down these issues into a logical, step by step process so that we all can follow.

## 10. Our focus today

We understand that accessibility can be a complex and difficult topic. So in this webinar, we will be focusing on the fundamental topics of accessibility, how to get started, and how we can take simple actions to identify accessibility issues. We will try not to dive deep into the code. But if you are a developer, we have two presentations about web accessibility at last year's Esri Developer Summit. We have posted links to the recordings in the Accessibility group on GeoNet.

We will give two presentations on web accessibility at this year's Developer Summit as well. So check out the schedule if you are interested.

## 11. Focus and tab order

### WCAG 2.4.7 Clear focus

Focus is the visual indicator that shows which control on the screen currently receives input from the keyboard. If users use keyboard to navigate a page, they should be able to see which control they are on at any time.

The best way to ensure clear focus is to have a visible border or outline around the element in use, whether it’s a form field, link, menu, content area or any other interactive element. This makes it easier for your users to understand where they are on a page.

Browsers have default styles for focus. We could customize the focus style if needed, but don't just disable the browser's default focus style.

### WCAG 1.3.2 Tab order

Tab order is the order in which focus proceeds forward and backward through interactive elements via the Tab key. As a keyboard user navigates through the page, the order in which interactive items receive keyboard focus is important.

The default keyboard navigation order must be logical and intuitive. For example, in English we read from left to right and from top to bottom. So the tab order should follow the visual flow of the page: left to right and top to bottom. And we should let the web page's source code determine the tab order.

I should point out that letting the keyboard focus jumping around on the page is not only an accessibility issue, but also a usability issue.

### WCAG 2.1.1 Keyboard access

Many people use keyboard to use a web page. Some of them may have motor impairment, and some may be power users that are faster with keyboard. Like mouse users, keyboard users should be able to use forms, menus, or any other functionalities on a web page.

### WCAG 2.1.2 Keyboard trap

A keyboard trap occurs when a user can get into a subsection on a web page by using the keyboard, but the user cannot get out of that subsection through the keyboard.

A common exception of this rule is when we show a modal dialog to the user, the dialog needs to trap keyboard focus until the user chooses to close the dialog. This is because the dialog introduces a new workflow to the user and needs the user's input to complete the new workflow.

## 16. Color and color contrast

### WCAG 1.4.1 Color only info

Users with visual impairment need help when we use color on the web. As many as 1 in 12 men have some degree of color blindness. That means about 8% of male users may struggle if we don't use color correctly. For example, if we use red text only to show an error message, users who cannot see red will not notice that message is an error. So that error message needs at least one more means to convey the meaning, like an error icon.

As another example, when we use color only to show different datasets in a chart, color blind users may not understand the different datasets. We should add clear labelling and patterns to those datasets, in addition to colors.

This guideline is not about removing color from our web pages or making web pages black and white, far from it. It just means that color should not be the only way of conveying information. Adding additional ways of conveying the same information in a lot of cases not only improves the accessibility, but also the overall user experience.

## 18. White text on colored background

When using white text on a colored background, it is sometimes hard to achieve a good contrast. You may be surprised how dark the color needs to be to meet the 4.5 contrast ratio. This can create hierarchy issues when those elements are not supposed to be the focus of the page - dark colored backgrounds will really grab the user's attention.

## 19. Flipping the contrast

You can solve the problem by flipping the contrast. Instead of using light text on a dark colored background, use dark colored text on a light colored background. The color is still there to help support the text, but it's way less prominent and does not interfere as much with other parts of the page.

### WCAG 1.4.3 Contrast ratio

All of us will benefit from a good contrast between text and its background color. For users with visual impairments, good contrast is essential.

## 21. Text alternatives

### WCAG 1.1.1 Text alternatives

Alternative (or 'alt') text is a text replacement for non-text content like images. Non-sighted users rely on the alternative text to understand information in images. When they use screen reader and encounter an image, the screen reader will announce the alt text of the image. If the image does not have alt text, the screen reader will usually announce the file name of the image, which is not useful.

A common exception for this guideline is that if an image is decorative and it does not convey meaning, we should set the alternative text to an empty string.

## 26. DIY accessibility test

So we recommend a four-step process to test accessibility of web applications. The four steps are automated test, keyboard test, screen reader test, and color test.

This is also the process we follow at Esri. It breaks down the testing to a logic flow, and it minimizes the switching between different types of tests that we need to do.