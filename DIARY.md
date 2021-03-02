# 2/8/21

## Index > Menu > ToDo

Today I am creating a menu for the index page. The menu items will be: Schedule a session; Blog; About; Contact. The menu will be hidden by default. When the page loads, a splash modal appears, enticing the first-time visitor to go deeper. The user may click on the central button, which brings up the About modal, or X out of the modal, which causes the menu to appear. The menu is not a modal - it's actually there. It appears with a right-to-left flipping animation suggesting a card flipping over. The menu has the same rounded border-radius as the modal, although it isn't necessarily in the same place on the screen. Some sort of razzle-dazzle happens when you mouse over the menu items. Not quite sure what yet - in the beginning it can be just a simple highlighting.

Ultimately, this website will be only one page, with a menu and five different possible modals: The splash modal appears upon page-load, and the other four modals appear when you click the corresponding button in the menu. 

Last night I changed the About page so that the content was in a card instead of a modal. I will need to undo that change. That's right: everything will be a modal. There will be a scheduler modal, a blog modal, a contact modal, an FAQ modal, and eventually maybe other modals as well. On the actual page there will only be a menu, whose job is to activate modals and which is hidden whenever there is an active modal.

The first task is to create the menu. I will begin by copy-pasting the entire container that I put my FAQ in last night and put it in the Index page, just to establish the space, and then convert it from a scrolling text body into a menu. The best way to do it would probably be with rows: One container, one row, four columns.

Not sure yet about colors and other razzle-dazzle. I do know that I want it to hide whenever a modal is active, and to appear and disappear with a flipping animation.

# 2/9/21

Today I will actually do what I said I was going to do yesterday. I will start by copy-pasting the content div from the about page.

# 2/10/21

Yesterday I did what I said I was going to do, although I forgot to document it. The index page now has a menu with four items. For the colors I just used Bootstraps built-ins. I've also incorporated a JQuery plugin that I will use to make the menu flip over like a card.

My current challenge is that I lost some styling, probably when I did the Git reset to change the content window on my about page back into a modal. I could root around in my Git log again to try and find it, but I think I'd rather just do it over.

Okay, now it looks pretty good. On load, I see a splash modal with buttons that bring up the about modal and the schedule modal. The menu appears and disappears with a card-flipping effect. Right now the effect is triggered with hover, which is not ideal and won't translate well to smartphone screens, but works for the time being. I still need to make the blog and contact modals, even if the former is for now just a placeholder. I also need to refine the card-flipping effect so it triggers based on whether or not there is an active modal. I also need to make everything look a little bit nicer. Aside from that, it's pretty much done!

TODO: 

-Turn the question mark div in the Splash modal into the button for the About modal. Get rid of the "learn more" button - instead, the "schedule a session" button should extend all the way across the modal, and the words "learn more" should appear on either side of the question mark. Not sure what color. Consider adding a flip effect on click.

-Pick one "schedule a session" button style.

-Make the X-out button look nicer.

-Figure out and fix the bug that makes the menu appear at the beginning.

## 3/2/21

Breaking news! I've decided to turn this website into a general-purpose portfolio page for myself. The title of the website will be "The Code Fool". The splash modal will have a picture of The Fool, and the quote from Blake. This may be my first branch!