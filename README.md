# Red Panda Gaming History

Red Panda Gaming History is a website that brings some gaming knowledge to you. These Infos range from the early games like Pong to AAA Games and the Games we have now. You will even see some of the biggest video game achievements. Come and learn a bit about Video Games [here](https://duudlez.github.io/Red-Panda-Gaming-History/)

## Features

### Site wide
* Navigation Menu
     * Contains links to  the Home, Gaming-History and Screenshots pages and will be responsive on all devices.
     * This will allow users to easily navigate between the pages on any size device.

![Nav Menu](docs/readme-images/Navbar.png)
* Footer
     * This will contain icons as links to social media websites that will open in new tabs. Icons will be accessible to the visually impaired who may be using a screen reader.
     * This will allow users to follow Red Panda Gaming History on various social media where they can stay up to date with Video Games.

![Footer](docs/readme-images/Footer.png)
* Favicon
     * A site wide red panda favicon will be implemented.
     * This will provide an image in the tabs header to allow the user to easily identify the website if they have multiple tabs open.

![Favicon](docs/readme-images/Favicon-readme.png)
* 404 Page
     * A 404 page will be implemented and will display if a user navigates to a broken link.
     * The 404 page will allow the user to easily navigate back to the main website if they direct to a broken link / missing page, without the need of the browsers back button.

![404](docs/readme-images/404-page.png)

### Landing Page
* Landing page image
     * This will be an image of a Red Panda sitting at a pc.
     * This will show the user that the Website is about pc's and gaming.


![Landing Page Image](docs/readme-images/landing-page.png)
* Website information on 'Red Panda'
     * Information about 'Red Panda' and the websites purpose.
     * This information let's the user know what the site is about.

![Bio](docs/readme-images/About-me.png)

* Contact form
     * A contact form will be implemented to allow users to contact 'Red Panda'. The form will consist of the following fields and attributes:
          * First Name (required, type=text)
          * Last Name (required, type=text)
          * Email (required, type=email)
          * Message (required, type=textarea)
    * On successful submission of the contact form, the user will be navigated to contact.html displaying a success message.
    * This will allow the user to contact 'Red Panda' if they have any questions or suggestions about Gaming History.

![Contact Form](docs/readme-images/Contact-Form.png)

![Contact Form Received](docs/readme-images/contact-form-received.png)

### Screenshots
* Screenshots
     * The screenshots section will provide the user with a small selection of Screenshots made by Red Panda and his Friends.
     * These screenshots show a few games Red Panda and his friends have played.

![Screenshots](docs/readme-images/screenshots.png)
<br><br><br><br>


## Technologies

* HTML
     * The structure of the Website was developed using HTML as the main language.
* CSS 
     * The website was styled using custom CSS in an external file.
* GitHub
     * Used as IDE and used to commit and push code during the developement of the Website.
* Font Awesome
     * Icons obtained from https://fontawesome.com/ were used to create the Social links in the footer.
* 11zon
     * (https://www.11zon.com/) was used to reduce the size of images used on the website
* Faicon.io
     * favicon files were created at https://favicon.io/favicon-converter/


## Testing

### Responsiveness

All pages were tested to ensure responsiveness on screen sizes from 320px and upwards.

Steps to test:

1. Open Browser an navigate to [Red Panda Gaming History](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Open the developer tools (right click and inspect)
3. Set to responsive and decrese width to 320px
4. Set the zoom to 50%
5. Click and drag the responsive window to maximum width

Expected:

Website is responsive on all screen sizes and no images are pixelated or stretched. No horizontal scroll is present. No elements Overlap.

Actual:

Website behaved as expected.

### Accessibility

[Wave Accessibility](https://wave.webaim.org/) tool was used throughout development and for final testing of the deployed website to check for any aid accessibility testing.

Testing was focused to ensure the following criteria were met:

- All forms have associated labels or aria-labels so that this is read out on a screen reader to users who tab to form inputs
- Color contrasts meet a minimum ratio as specified in [WCAG 2.1 Contrast Guidelines](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html)
- Heading levels are not missed or skipped to ensure the importance of content is relayed correctly to the end user
- All content is contained within landmarks to ensure ease of use for assistive technology, allowing the user to navigate by page regions
- All not textual content had alternative text or titles so descriptions are read out to screen readers
- HTML page lang attribute has been set
- Aria properties have been implemented correctly
- WCAG 2.1 Coding best practices being followed

### Lighthouse Testing

![Home](docs/readme-images/index-lighthouse.png)

![Screenshots](docs/readme-images/screenshots-lighthouse.png)

![Gaming-History](docs/readme-images/gaming-history-lighthouse.png)

### Functional Testing

**Navigation Links**

Testing was performed to ensure all navigation links on the respective pages navigated to the correct pages as per design. This was done by clicking on the naviigation links on each page.

| Navigation Link | Page to Load        |
| --------------- | ------------------- |
| Home            | index.html          |
| Gaming History  | gaming-history.html |
| Screenshots     | gscreenshots.html   |

Links on all pages navigated to the correct pages as expected.

**Form Testing**

The form on the home page was tested to ensure it funtioned as exected when correct data was input an when incorrect data was input. The following scenarios were covered:

_Scenario One - Correct Inputs_

Steps to test:

1. Navigate to [Red Panda Gaming History - Home Page](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Scroll down to the form and input the following data:
   - First Name: John
   - Last Name: Doe
   - Email: john.doe@test.de
   - Comment: This is a test.
3. Click Submit
4. User should be redirected to contact.html confirmation page

Expected: 

Form submits with no warnings or errors and user is redirected to contact.html confirmation page.

Actual:

Website behaved as expected with no error or warnings and redirected to contact.html confirmation page.

_Scenario Two - Missing Required Field First Name_

Steps to test:

1. Navigate to [Red Panda Gaming History - Home Page](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Scroll down to the form and input the following data:
   - First Name:
   - Last Name: Doe
   - Email: john.doe@test.de
   - Comment: This is a test.
3. Click Submit

Expected:

The form does not submit and an Error is displayed to tell the user that the field is required.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

_Scenario Three - Missing Required Field Last Name_

Steps to test:

1. Navigate to [Red Panda Gaming History - Home Page](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Scroll down to the form and input the following data:
   - First Name:John
   - Last Name:
   - Email: john.doe@test.de
   - Comment: This is a test.
3. Click Submit

Expected:

The form does not submit and an Error is displayed to tell the user that the field is required.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

_Scenario Four - Missing Required Field Email_

Steps to test:

1. Navigate to [Red Panda Gaming History - Home Page](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Scroll down to the form and input the following data:
   - First Name:John
   - Last Name: Doe
   - Email:
   - Comment: This is a test.
3. Click Submit

Expected:

The form does not submit and an Error is displayed to tell the user that the field is required.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

_Scenario Five - Incorrect email format_

Steps to test:

1. Navigate to [Red Panda Gaming History - Home Page](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Scroll down to the form and input the following data:
   - First Name:John
   - Last Name: Doe
   - Email: john.doetest.de
   - Comment: This is a test.
3. Click Submit

Expected:

The form does not submit and an Error is displayed to tell the user that a valid email is required and the format it should be in.

Actual:

Website behaved as expected, error message was displayed and the form did not submit.

**Footer Social Media Icons / Links**

Testing was performed on the Font Awesome Social Media icons in the footer to ensure that each one opened in a new tab and that each one had a hover affect of the orange branding color.

Each item opened a new tab when clicked as expected and correct hover color was present.

**Footer Contact Information**

Testing was performed on the phone number in the contact information section of the footer to ensure behaviour was as expected.

_Steps to test Telephone Number_

1. Navigate to [Red Panda Gaming History - Home Page](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Click the phone number in the footer (00 123 456 789)

Expected:

A window is opened asking which device you would like to call from.

Actual:

Behavior was as expected and the window presented me with the option to call.

_Steps to test Email Link_

1. Navigate to [Red Panda Gaming History - Home Page](https://duudlez.github.io/Red-Panda-Gaming-History/)
2. Click the email address in the footer (rpgh@gmail.com)

Expected:

A windows popup is displayed asking what application you would like to send a mail from or your default email application is opened.

Actual:

Behavior was as expected and my outlook application was opened ready to send an email to the target address.

### Validator Testing

- HTML
  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org)

![Contact HTML Validator Results](docs/testing/validator-testing-contact.png)

![Gaming-History HTML Validator Results](docs/testing/validator-testing-gaming-history.png)

![Home HTML Validator Results](docs/testing/validator-testing-index.png)

![Screenshots HTML Validator Results](docs/testing/validator-testing-screenshots.png)

![404 HTML Validator Results](docs/testing/validator-testing-404.png)

- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org)

![CSS Validator Results](docs/testing/css-validator.png)

## Deployment

### Version Control

The site was created using the Visual Studio code editor and pushed to github to the remote repository ‘Red-Panda-Gaming-History’.

The following git commands were used throughout development to push code to the remote repo:

```git add <file>``` - This command was used to add the file(s) to the staging area before they are committed.

```git commit -m “commit message”``` - This command was used to commit changes to the local repository queue ready for the final step.

```git push``` - This command was used to push all committed code to the remote repository on github.

### Deployment to Github Pages

- The site was deployed to GitHub pages. The steps to deploy are as follows: 
  - In the GitHub repository, navigate to the Settings tab 
  - From the menu on left select 'Pages'
  - From the source section drop-down menu, select the Branch: main
  - Click 'Save'
  - A live link will be displayed in a green banner when published successfully. 

The live link can be found here - https://duudlez.github.io/Red-Panda-Gaming-History/

### Clone the Repository Code Locally

Navigate to the GitHub Repository you want to clone to use locally:

- Click on the code drop down button
- Click on HTTPS
- Copy the repository link to the clipboard
- Open your IDE of choice (git must be installed for the next steps)
- Type git clone copied-git-url into the IDE terminal

The project will now of been cloned on your local machine for use.

## Credits

* Some Screenshots used are from a Friend. Permission was granted to use them on my Website.
* [Microsoft Designer](https://designer.microsoft.com/)
     * Favicon, Hero Image and Pictures on the Gaming History site were created using Microsoft Designer.
