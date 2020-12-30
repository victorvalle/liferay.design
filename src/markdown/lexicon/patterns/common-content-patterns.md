---
title: 'Common Content Patterns'
description: 'Spectrum of different content situations in our interfaces.'
order: 132
draft: false
---

import { Grid, Box } from 'theme-ui'

<div class="adapting-columns">
    <p><a href="./#confirmation--acknowledgement">Confirmation & Acknowledgement</a></p>
    <p><a href="./#titles">Titles</a></p>
    <p><a href="./#lists">Lists</a></p>
    <p><a href="./#links">Links</a></p>
    <p><a href="./#dropdown-menus">Dropdown menus</a></p>
    <p><a href="./#bad-news">Bad News</a></p>
    <p><a href="./#errors">Errors</a></p>
    <p><a href="./#empty-states">Empty states</a></p>
    <p><a href="./#buttons">Buttons</a></p>
    <p><a href="./#modal">Modal</a></p>
    <p><a href="./#descriptions">Descriptions</a></p>
    <p><a href="./#instructions">Instrunctions</a></p>
    <p><a href="./#alerts">Alerts</a></p>
</div>
<br/>
<br/>
<br/>

### Confirmation & Acknowledgement

Confirmation and acknowledgement helps reduce uncertainty for actions a user has taken or is about to make.

#### Confirmation

**When to use it**

Confirmation messages should be used when the user's action will result in a critical situation. There are two main use cases to consider:

* A risk action: The action the user is going to perform has significant consequences that can't be undone or easily undone. Ex: site deletion.
* An unintended consequence: The action the user is taking has notable side effects that may leave them feeling disoriented. Ex: a site switch that results in a complete change of context, including user permissions.

Confirmation messages are rarely needed and should only be used when they fall under one of the two cases mentioned above.

<br />
<br />

**When do avoid it**

Providing extremely clear feedback can prevent the need for confirmation messages. Do not use a confirmation message for the following cases:

* Error prevention: The interface should clearly communicate its intended use, thus preventing the need for a confirmation message to communicate potential errors.
* Undo actions: If an action has an undo action, you must never use a confirmation message to proceed with the action. A clear example is “Move to Recycle Bin”.
* Unless a confirmation message is absolutely required, as explained in the previous section, do not use one.

<br />
<br />

**How to write a confirmation message**

Your confirmation message must clearly communicate the situation and the potential results of proceeding with the action. An unclear message can result in the user mistakenly taking irreversible actions or finding themselves in an unexpected situation.

Follow these guidelines to write a good confirmation message:

* Do not write generic and open questions. Ex: Are you sure?
* Be clear and concise.
* Provide exact information to your user, so there is no uncertainty on the action to be confirmed.
* If the confirmation initiates an action, the label of the button to confirm should contain the verb associated with the action.
* If the confirmation is informational in nature, there should only be a “Ok” button.
* Address your questions and statements so they can be easily answered with "Ok" and "Cancel", as they are provided by the browser.

<br />
<br />

_Image_

_Image_

_Image_

<br />
<br />

**Implementation**

Confirmation messages are browser native. Therefore, Lexicon does not style them. Browser native confirmation messages are accessible and work perfectly on every device.

#### Acknowledgment

Acknowledgments are accomplished with toasts type of alerts. They should plainly state the action that was taken. Acknowledgements occur along with a confirmation and sometimes when an action occurs in the background.


<br />
<br />

<Grid variant='smallCards' >
	<Box>
		<p class="example-text">List was successfully saved.</p>
		<br />
		<p class="do">Do</p>
	</Box>
	<Box>
		<p class="example-text"><a class="example-text link-false">John.doe@liferay.com</a> was added to this list.</p>
		<br />
		<p class="dont">Don't</p>
	</Box>
</Grid>


### Titles

Titles should use sentence casing.

<br />
<br />

<Grid variant='smallCards' >
	<Box>
		<p class="example-text">Select file</p>
		<p class="example-text">Assign users to this site</p>
		<p class="example-text">Select site or asset library</p>
		<br />
		<p class="do">Do</p>
	</Box>
	<Box>
		<p class="example-text">Select File</p>
		<p class="example-text">Assign Users to This Site</p>
		<p class="example-text">Select Site or Asset Library</p>
		<br />
		<p class="dont">Don't</p>
	</Box>
</Grid>


### Lists 

To adhere to Chicago Manual of Style guidelines, we should always include a colon to introduce any bullet points.

Full sentences require proper formatting including punctuations.

<br />

<Grid variant='smallCards' >
	<Box>
		<p class="example-text">Benefits of upgrading:</p>
        <ul>
            <li class="example-text">Get setup faster with a one step connection process.</li>
            <li class="example-text">Secure your connection using blockchain technology.</li>
            <li class="example-text">Control the data you want to send.</li>
        </ul>
	</Box>
</Grid>
<br />


If they are fragments, no punctuation required. However, they should adhere to sentence casing rules. 

<br />

<Grid variant='smallCards' >
	<Box>
		<p class="example-text">Benefits:</p>
        <ul>
            <li class="example-text">Faster setup</li>
            <li class="example-text">More secure</li>
            <li class="example-text">Finer control of your data</li>
        </ul>
	</Box>
</Grid>

<br />


Use parallel construction 

<br />

<Grid variant='smallCards' >
	<Box>
		<p class="example-text">What to bring:</p>
        <ul>
            <li class="example-text">Fruits</li>
            <li class="example-text">Wine</li>
            <li class="example-text">Spreads</li>
            <li class="example-text">Blanket</li>
            <li class="example-text">Sunblock</li>
        </ul>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
		<p class="example-text">What to bring:</p>
        <ul>
            <li class="example-text">Fruits</li>
            <li class="example-text">Wine</li>
            <li class="example-text">Spreads</li>
            <li class="example-text">A blanket incase its cold</li>
            <li class="example-text">Sunblock</li>
        </ul>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />
<br />

<Grid variant='smallCards' >
	<Box>
		<p class="example-text">Rules to stay safe:</p>
        <ul>
            <li class="example-text">Don’t feed wildlife</li>
            <li class="example-text">Explore in pairs</li>
            <li class="example-text">Use trash cans</li>
            <li class="example-text">Respect your neighbors</li>
        </ul>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
		<p class="example-text">Rules to stay safe:</p>
        <ul>
            <li class="example-text">Don’t feed wildlife</li>
            <li class="example-text">Explore in pairs</li>
            <li class="example-text">Trash cans should be used</li>
            <li class="example-text">Respect your neighbors</li>
        </ul>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />
<br />

Avoid using the same first word:

<br />

<Grid variant='smallCards' >
	<Box>
        <ul>
            <li class="example-text">Enjoy yourself</li>
            <li class="example-text">Have an adventure</li>
            <li class="example-text">Build teamwork</li>
        </ul>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <ul>
            <li class="example-text">It will be fun</li>
            <li class="example-text">It will an adventure</li>
            <li class="example-text">It will teach you team building </li>
        </ul>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>


### Links 

Make sure to include nouns (the thing it is linking to)

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Policy Details</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Review</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />


Consider accessibility. Imagine listening to a list of links on the page. Would you know where it goes next without contextual clues?

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Policy Details</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Details</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />

### Dropdown menus  

* Limit to a single line of text
* Action menus (kebab menu) - use verbs
* Navigational menus - use nouns

### Bad news

Bad news refers to situations where Liferay must deliver unwelcomed news.

* Client’s payment issues
* Cancellation of a scheduled event
* A feature that is not supported by legacy versions of Portal
* Sunset support of a version/feature

Our advice is to:

* Be direct about the bad news
* Be positive
* Focus on the solution
* Avoid you, your pronouns
* Be transparent without self-blaming. If an apology is in order, apologize for the negative effect, rather than what we did wrong. Apologize when something we did, causes more work for the customer.

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">This version of the portal is no longer being supported. Good news, we have a wealth of 6.2 resources in our archives.</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">You have an outdated version of the portal and we don’t offer support for 6.2.</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />

### Errors

Error messages should reinforce trust in the product, without losing momentum in the task at hand. The goal is to build trust with each error message, however an error free experience is the goal.

* Describe the problem specifically
* Maintain momentum
* Be brief and simple
* Offer more information when necessary
* Provide recovery solutions


#### Error recovery 

Prevent the same message from reappearing
* Supply enough information to minimize mistakes
* Providing examples with hints or explicit help to eliminate the possibility of errors.
* Have a call to action or describe how to progress
* If the same error is triggered 2+ times, consider another way to progress.

Be given in real time (ie: in forms, in call to actions)
* Inform about valid format rules

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">There are conflicting rules for your data request. Remove the conflict (a) or (b) and try again.</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Oops there is an error in your data request.</p>
        <p class="example-text">Oops there is an error in your data request. It’s probably very easy to resolve. Please refer to our documentation to find the resolution.</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />

#### Unknown error

Sometimes there is an unknown error caused by something technical. Do not use the technical error provided by the back end. Do not try to explain the situation.

Recommended unknown error message: 

<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">“Something went wrong, try again.”</p>
	</Box>
</Grid>

<br />


### Empty states

Empty states, similar to errors, are an opportunity to build trust.

* Be clear and concise
* Use positive language
* Offer a call to action

<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">You’re done with all your tasks. Create a new task?</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">You don’t have any more tasks left.</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />
<br />

Sometimes empty states do not depend on user actions. In these cases, offer a clear and concise description.

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">There are no search terms for this period.</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">No data</p>
        <p class="example-text">We’re collecting search data, but there is nothing yet.</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />

Empty state example

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Image</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Image</p>
        <p class="example-text">Image</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />



### Buttons

Should be title cased - we want to bring more attention to the actions provided by buttons. Title casing buttons also provide subtle affordance to borderless buttons. 

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Image</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Image</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />

Button text should be specific to the action that the button is performing.

* Use verbs that indicates the action
* “New” can be used as a verb, this is an exception to this rule.


### Modal

When a modal contains an action, the action should be in both the title and the call to action. 

* Title: Delete workspace
* CTA: Delete

_Image_

_Image_

_Image_

An object related modal, does not require a title.

_Image_


### Descriptions

Sometimes descriptions are necessary to describe what the feature will help the user accomplish. Typically found during configuration, stepped walk throughs, forms, and settings screens.

Descriptions should be human/use-case centered rather than software centered.

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Define an experience for XYZ segment by selecting contacts and content.</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Selecting contacts and content sets will dynamically change page content whenever analytics.load function is called by the API. </p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />

Boolean situations are those yes/no situations usually solved with checkboxes.
* Be as explicit as possible to let the use know the the impact of their decision
* Do not hide helpful information in popovers, alerts, or secondary text.

_IMAGE_

Trying to avoid:

_IMAGE_


Practice progressive disclosure

* Reveal information as needed. For example don’t over complicate things by worrying about what could happen down the line. Rather, explain the situation at the point of intention.

_IMAGE DO_

_IMAGE DONT_

For the remaining text “Inactive events will automatically be set to hidden after 30 days of inactivity and removed if inactive for the duration for the retention period.” 

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Display tooltip on hover over an inactive events and in the instructions under event settings.</p>
	</Box>
</Grid>

<br />


### Instructions

Instructions are explanations that guide the user towards an action.

Practice progressive disclosure

<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Select a training period</p>
        <br />
        <p class="example-text">Select items for training. Only items with interactions during the set period are available for selection.</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Select a training period, this will inform what items are available for the current training period.</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />

When referring to a UI element, use the casing of the element on screen, there is no need to emphasize otherwise with bold, italics or a combination of both.

_IMAGE_


### Alerts



<br />
<br />

<Grid variant='smallCards' >
	<Box>
        <p class="example-text">Select a training period</p>
        <br />
        <p class="example-text">Select items for training. Only items with interactions during the set period are available for selection.</p>
        <br />
		<p class="do">Do</p>
	</Box>
    <Box>
        <p class="example-text">Select a training period, this will inform what items are available for the current training period.</p>
        <br />
		<p class="dont">Don't</p>
	</Box>
</Grid>

<br />