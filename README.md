# cld-cropping-intro

This microcourse dives into the diverse world of automatic image cropping with Cloudinary. Learners will be introduced to the plethora of cropping methods available with Cloudinary, understanding their unique applications and limitations. 

Explore the intricacies of aspect ratios and the importance of considering various viewports or device screen sizes for responsive design.

Discover the concept of gravity in Cloudinary, and illustrate its role in determining the focal point of cropped images. Additionally, learners will gain insight into automatic cropping (c_auto), its benefits, and practical application.

Through hands-on code examples, learners will discover how to apply automatic cropping (c_auto) and leverage automatic gravity detection (g_auto), or specify specific gravity locations like g_dog or g_face. By the end of the microcourse, participants will be equipped with the knowledge and skills to effectively crop images in diverse scenarios, optimizing them for different contexts and devices.

## Environment Setup

### Install Node.js and NPM:
You will need to install Node.js on your machine, version 10 or higher.
 Important - Installing Node.js will also install npm, the package manager for Node.js.

#### Mac Users
Using Homebrew:

```bash
brew install node
```

#### Windows
[Download for windows](https://nodejs.org/en/download/)

#### Verify Node/NPM install:

```console
$ node --version
v18.18.1

$ npm --version
9.8.1
```

### Choose an IDE or Use Text Editor:

- [Visual Studio Code](https://code.visualstudio.com/download) - VSCode is our preferred IDE
- [WebStorm](https://www.jetbrains.com/webstorm/) 
- [Sublime](https://www.sublimetext.com/) 
- [Atom](https://atom.io/) 
- [iTerm](https://iterm2.com/) 

### Download Repository:

[Introduction to Cropping Essentials: Maximizing Efficiency with Cloudinary](https://github.com/cloudinary-training/cld-cropping-intro)

- Run code from root directory, like so:
```bash
node <file_name.js>
```


### Account Setup and Credentials:

1. If you don't have one already, create a free Cloudinary account at: https://www.cloudinary.com/signup.

2. Navigate to the Dashboard. Copy the `CLOUDINARY_URL` into your clipboard (see yellow arrow).

![Dashboard](./assets/environment_variable.png)

3. Create a `.env` file in the root of the project. Paste the CLOUDINARY_URL environment variable into your `.env` file.

There should be one line of code in your .env file, which should look like this:

```console
CLOUDINARY_URL=cloudinary://YOUR_API_KEY:YOUR_API_SECRET@YOUR_CLOUD_NAME
```
- Key: CLOUDINARY_URL
- Value: cloudinary://API_KEY:API_SECRET@CLOUD_NAME

Doing this step properly is essential, as it will let Cloudinary know who you are and provide access to your cloud.

### Run Code: Install Node Libraries


```console
npm i
```
(You will be using the `cloudinary` and the `dotenv` libraries.)

### Run Code: Test Credentials

```console
node testCredentials.js
```

The output should look like this:
```console
your Cloud Name
your API Key
```

- Your API_SECRET is part of your CLOUDINARY_URL
- Remember to always keep your API_SECRET a secret!
  - This is why we programmed testCredentials.js to only output your cloud name and API Key (no need to keep these two credentials private)


### Run Code:

In order to upload all of the assets associated with these code examples and assign the correct Public ID to each, run this file:
```bash
node upload.js
```

Now you're ready to get started! 


### Helpful Cloudinary Docs, Demos, and Tutorials:
- [Resize and Crop Modes](https://cloudinary.com/documentation/resizing_and_cropping#resize_and_crop_modes)
- [c_auto](https://cloudinary.com/documentation/transformation_reference#c_auto)
- [c_auto demo](https://cloudinary.com/demo/c_auto)
- [Aspect Ratio](https://cloudinary.com/documentation/transformation_reference#ar_aspect_ratio)
- [Image Resizing and Cropping](https://cloudinary.com/documentation/resizing_and_cropping#automatic_gravity_with_the_auto_cropping_mode)
- [Face-detection Based Cropping](https://cloudinary.com/documentation/face_detection_based_transformations#face_detection_based_cropping)
- [Cloudinary AI Content Analysis Add-On](https://cloudinary.com/documentation/cloudinary_ai_content_analysis_addon)
- [Gravity Feature](https://cloudinary.com/documentation/transformation_reference#g_gravity)
- [Gravity Positions for Crops](https://cloudinary.com/documentation/resizing_and_cropping#control_gravity)
