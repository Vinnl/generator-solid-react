# Solid React Application Generator

## 0.6.2 (September 11, 2019)

#### Solid React Application Base

##### Updated
* Updated dependency packages to fix security vulnerabilities

## 0.6.1 (August 28, 2019)

#### Generator

##### Added
* New prompt when creating a new application. The new prompt asks if the developer would like to install a full sample application or just a simple one-page application. This provides a way for people familiar with Solid to create new blank applications and get started quicker.

## 0.6.0 (August 14, 2019)

#### Solid React Application Base

##### Added
* New Tic-Tac-Toe Game
  * Demonstrates key Solid functionality such as:
      * Discovering where a user wants their application data to be stored
      * Creating application-specific files and folders
      * Managing permissions of files and folders
      * Discovering a global inbox
      * Sending game invite notifications to a global inbox
      * Creating and/or discovering an application-specific inbox
      * Sending application-specific notifications to the application inbox
      * Granting access to different Pods, to allow opponents to read data from and write data to your Pod
      * Interoperable notification data structure, so notifications in the global inbox can be read by any compatible application

## 0.5.2 (June 19, 2019)

#### Solid React Application Base

##### Updated
* Latest version of solid-react-components
* Error toast messages must now be manually dismissed

##### Fixed
* Fixed some missing error translations

## 0.5.1 (June 5, 2019)  

#### Solid React Application Base

##### Updated
* Profile form now autosaves
* Profile form now liveupdates when the form data changes from another source
* New error messages (and translations) added for the new profile form
* Latest version of solid-react-components

##### Fixed
* Login Provider list is now properly left-aligned instead of center-aligned
* Registration page title is now the proper color and is no longer underneath the top nav
* Profile image predicate now matches the Solid data browser profile image predicate
* Uploading multiple profile images from the welcome page now properly uses the latest uploaded file (previously was only using first uploaded file)


## 0.5.0 (May 22, 2019)

#### Solid React Application Base

##### Updated
* Major reworking of profile page
  * Profile form is now automatically generated from a ShEx shape
  * LiveUpdate capabilities are temporarily removed from the profile page. This functionality is being moved to the ShexFormBuilder component in a future release
  * ShEx shape has been created to match with the data browser. This means there are a lot of new fields and changed predicates in the profile
  * Link to [userprofile.shex](https://shexshapes.inrupt.net/public/userprofile.shex) shape added to demonstrate consuming and hosting a ShEx shape

##### Fixed
* Fixed npm vulnerabilities ([#165](https://github.com/inrupt/generator-solid-react/issues/165))
* Resolved issue where npm install was hanging on certain packages ([#164](https://github.com/inrupt/generator-solid-react/issues/164))

## 0.4.2 (April 17, 2019)

#### Solid React Application Base

##### Updated
* Changed favicon
* Version number increment for the Solid Style Guide
* Changed the name of the SDK across the site to "Solid React SDK by inrupt"

##### Fixed
* Form placeholder text now properly translates to Spanish
* Responsive top navbar is more consistent in when it appears
* Language selection dropdown now appears in the responsive top navbar when the user is not logged in
* [FireFox] Responsive top navbar menu hover state is position properly
* [Safari] Responsive top navbar hamburger menu list now displays properly


## 0.4.1 (April 4, 2019)

#### Solid React Application Base

##### Added
- Profile page now receives updates in real time. If you change your profile elsewhere, such as the data browser, the profile page will immediately be updated to reflect those changes
- Language Selection dropdown now includes flag icons

##### Removed
- Welcome page no longer has a logout button

##### Fixed
- Max image size is now displayed in the error message displayed when the size is exceeded
- Profile image in top nav is now updated immediately when a new profile image is uploaded
- Footer now has a mobile-friendly display when resolution is too low

## 0.4.0 (March 20, 2019)

#### Solid React Application Base

##### Added
- Incorporated LDFlex data writing examples
- Profile Page
  - View Profile
  - Edit Profile
- Site Footer
  
##### Updated
- Made some adjustments to prepare for [React Hooks](https://reactjs.org/docs/hooks-intro.html) support
- Created environment file to store branding-specific variables. This should make it easier to change the branding on generated applications

##### Fixed
 - Toast messages now close when the site's language changes, to prevent confusion
 - Added some form validation to the profile form

## 0.3.0 (March 6, 2019)

#### Solid React Application Base

##### Added
- Internationalization support using [react-i18next](https://react.i18next.com/). This includes resource files for English and Spanish languages
- Language selection dropdown added to top navigation bar
- Ability to edit and upload a new profile image

##### Updated
- Solid Style Guide has been updated to the most recent version
- Solid React Components library has been updated to the most recent version
- Several changes to existing Solid React Components, such as new added parameters

## 0.2.1 (February 20, 2019)

#### Generator

##### Removed

- Deleted the default .yo-rc file, as it was not required by the generator

#### Solid React Application Base

##### Added

- Loading animation

##### Updated

- Dropdown menu for logout and profile
- Updated style guide to the latest version
- Solid React Components updated to v0.2.3

##### Fixed

- Minor style tweaks
- Welcome page image no longer becomes an oval on tall images
- Fixed notification display so it properly uses the title and content fields
- Error message is cleared when switching between provider login and webID login
- Login error text has been updated to add clarity

## 0.1.1 (February 5, 2019)

#### Solid React Application Base

##### Changed

- Updated Welcome Page text to be more clear and concise

## 0.1.0 (January 30, 2019)

### First Release

#### Generator

##### Added

- Generator created using [yeoman-generator](https://github.com/yeoman/generator-generator)
- First version of yeoman application configuration
- Added voca as a dependency to handle casing properly for app name

#### Solid React Application Base

##### Added

- Built scaffolded app with create-react-app, ejected to allow change in webpack configurations
- [LDFlex for Solid](https://github.com/solid/query-ldflex) added as the primary interface for most Linked Data operations
- Dependencies from [Solid React SDK](https://github.com/inrupt-inc/solid-react-sdk):
  - [Atomic Style Guide for Solid](https://github.com/Inrupt-inc/inrupt-atomic-styleguide) to provide global styling
  - [Solid React Components Library](https://github.com/Inrupt-inc/solid-react-components) to provide reusable core functionality
- [Styled Components](https://www.styled-components.com/) added as dependency to handle layout and custom styling
- Basic and Authenticated Nav Bar
- Login page
- Register page
- Not Found Page (404)
- Error handling
- Error page
- Test Infrastructure
- Unit testing for all components
