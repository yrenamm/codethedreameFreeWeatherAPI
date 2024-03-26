# Tests for Website Functionality

# Table of Contents

- [Tests for Website Functionality](#tests-for-website-functionality)
  - [Navigation](#navigation)
    - [Scenario: Navigate to Welcome Page](#scenario-navigate-to-welcome-page)
    - [Scenario: Return to Welcome Page from the other pages](#scenario-return-to-welcome-page-from-the-other-pages)
    - [Scenario: Return to Welcome Page from the other pages](#scenario-return-to-welcome-page-from-the-other-pages-1)
    - [Scenario: Return to Current Weather page from the other pages](#scenario-return-to-current-weather-page-from-the-other-pages)
    - [Scenario: Return to Historical Data page from the other pages](#scenario-return-to-historical-data-page-from-the-other-pages)
    - [Scenario: Access API Documentation](#scenario-access-api-documentation)
  - [Internationalization](#internationalization)
    - [Scenario: Change Language on Welcome Page](#scenario-change-language-on-welcome-page)
    - [Scenario: Change Language on Welcome Page to Russian](#scenario-change-language-on-welcome-page-to-russian)
    - [Scenario: Change Language on Welcome Page to Hebrew](#scenario-change-language-on-welcome-page-to-hebrew)
    - [Scenario: No Language Buttons on Non-Welcome Pages](#scenario-no-language-buttons-on-non-welcome-pages)
  - [Footer Links](#footer-links)
    - [Scenario: Open and Close Privacy Policy iFrame from Footer Link](#scenario-open-and-close-privacy-policy-iframe-from-footer-link)
    - [Scenario: Open and Close Contact Alert from Footer Link](#scenario-open-and-close-contact-alert-from-footer-link)
  - [Functionality](#functionality)
    - [Scenario: Access Current Weather Details](#scenario-access-current-weather-details)
    - [Scenario: Access Historical Weather Details](#scenario-access-historical-weather-details)
  - [Minor Details](#minor-details)
    - [Scenario: View Moving Gallery on Current Weather page](#scenario-view-moving-gallery-on-current-weather-page)
    - [Scenario: View Banner on Historical Data page](#scenario-view-banner-on-historical-data-page)
    - [Scenario: View Today's Weather area on Current Weather page](#scenario-view-todays-weather-area-on-current-weather-page)
    - [Scenario: View Today's Weather area on Current Weather page](#scenario-view-todays-weather-area-on-current-weather-page-1)


## Navigation

### Scenario: Navigate to Welcome Page
- **Given** the user opens the website [https://yrenamm.github.io/](https://yrenamm.github.io/)
- **When** the user navigates to the Welcome Page
- **Then** the Welcome Page should be displayed

### Scenario: Return to Welcome Page from the other pages 
- **Given** the user is on any page of the website
Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather)
- **When** the user clicks on the home button
- **Then** they should be redirected to the Welcome Page

### Scenario: Return to Welcome Page from the other pages 
- **Given** the user is on any page of the website
Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather)
- **When** the user clicks on the cloud icon
- **Then** they should be redirected to the Welcome Page
 
### Scenario: Return to Current Weather page from the other pages 
- **Given** the user is on any page of the website
Welcome page [https://yrenamm.github.io/](https://yrenamm.github.io/)
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather)
- **When** the user clicks on the Current Weather
- **Then** they should be redirected to the Current Weathere page

### Scenario: Return to Historical Data page from the other pages 
- **Given** the user is on any page of the website
Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather)
- **When** the user clicks on the Historical Data
- **Then** they should be redirected to the Historical Data page

### Scenario: Access API Documentation
- **Given** the user is on any page of the website
Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather)
- **When** the user clicks on the API Documentation link
- **Then** they should be redirected to the Open Meteo API documentation [https://open-meteo.com/en/docs](https://open-meteo.com/en/docs) (opens in a new tab)

## Internationalization 

### Scenario: Change Language on Welcome Page
- **Given** the user is on the Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/) 
- **When** the user clicks on the language button for English
- **Then** the main article should be displayed in English

### Scenario: Change Language on Welcome Page to Russian
- **Given** the user is on the Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
- **When** the user clicks on the language button for Russian
- **Then** the main article should be displayed in Russian

### Scenario: Change Language on Welcome Page to Hebrew
- **Given** the user is on the Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
- **When** the user clicks on the language button for Hebrew
- **Then** the main article should be displayed in Hebrew

### Scenario: No Language Buttons on Non-Welcome Pages
- **Given** the user is on a page other than the Welcome Page
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather)
- **When** the user views the page
- **Then** the language buttons should not be visible

## Footer Links

### Scenario: Open and Close Privacy Policy iFrame from Footer Link
- **Given** the user is on any page of the website
Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather
- **When** the user clicks on the Privacy Policy link in the footer
- **Then** an iFrame containing the Privacy Policy should be displayed
- **And** a close button should be available within the iFrame
- **When** the user clicks on the close button within the iFrame
- **Then** the iFrame containing the Privacy Policy should be closed

### Scenario: Open and Close Contact Alert from Footer Link
- **Given** the user is on any page of the website
Welcome Page [https://yrenamm.github.io/](https://yrenamm.github.io/)
Current Weather page [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html)
Historical Data page [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather
- **When** the user clicks on the Contact Me link in the footer
- **Then** a pop-up alert with the email address to contact should be displayed
- **And** a close button should be available within the pop-up alert
- **When** the user clicks on the close button within the pop-up alert
- **Then** the pop-up alert should be closed

## Functionality    

### Scenario: Access Current Weather Details
- **Given** the user is on the Current Weather Page or clicks on [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html) or the user clicks on the Current Weather link
- **When** the user selects each city from the dropdown one by one
- **And** submits the form
- **Then** the temperature and wind speed for the selected city should be displayed

### Scenario: Access Historical Weather Details
- **Given** the user is on the Current Weather Page or clicks on [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather.html) or the user clicks on the Historical Data link
- **When** the user selects each city from the dropdown one by one
- **And** submits the form
- **Then** the temperature of every hour for each selected city should be displayed as a table

## Minor Details

### Scenario: View Moving Gallery on Current Weather page
- **Given** the user is on the Current Weather page, or clicks on [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html), or the user clicks on the Current Weather link
- **When** the user views the page
- **Then** the moving gallery should be visually appealing and smoothly transition between images

### Scenario: View Banner on Historical Data page
- **Given** the user is on the Historical Weather Page, or clicks on [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather.html), or the user clicks on the Historical Data link
- **When** the user views the page
- **Then** the banner should be visually appealing and appropriately displayed

### Scenario: View Today's Weather area on Current Weather page
- **Given** the user is on the Current Weather page, or clicks on [https://yrenamm.github.io/currentWeather.html](https://yrenamm.github.io/currentWeather.html), or the user clicks on the Current Weather link
- **When** the user views the page
- **Then** the Today's Weather area should look good by usage Bootstrap from CDN

### Scenario: View Today's Weather area on Current Weather page
- **Given** the user is on the Current Weather page, or clicks on [https://yrenamm.github.io/historicalWeather.html](https://yrenamm.github.io/historicalWeather.html), or the user clicks on the Historical Data link
- **When** the user views the page
- **Then** the Historical Weather area should look good by usage Bootstrap from CDN