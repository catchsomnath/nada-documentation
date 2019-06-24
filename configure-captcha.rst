Configure Captcha
########################

NADA includes a built-in image captcha and also the Google Recaptcha v2. 

Using builtin Image Captcha
------------------------------

1. Edit the configuration file **application/config/captcha.php**.

2. Change the config option on **line 12** to **image_captcha**.

.. image:: images/captcha_options.png

3. Save the file.

4. To test, go to the login page and click on the **Register** link and you should see the Recaptcha visible at the bottom of the User Registration form.


Using Google Recpatcha v2
------------------------------

To use Google Captcha please follow the steps given below:

1. To use the Google Recaptcha, you'll need to generate the public/private keys using the google recaptcha website. 

2. Visit the Google Recaptcha website - https://www.google.com/recaptcha

3. Login to the website, or sign up. 

4. Once you have logged in, go to the Admin console to **Register a new site** or visit https://www.google.com/recaptcha/admin/create

.. image:: images/create_google_captcha.png
    :class: img-responsive

    
a. Provide a Label.

b. For ReCaptcha type, choose **reCaptcha v2** > **"I'm not a robot" Checkbox** option. 

c. Submit the form, which will open a confirmation page with the **Site Key** and **Secret Key**. We will need the keys to be added to the NADA configurations for ReCaptcha.
    
 
5. Edit the NADA configuration file ``application/config/captcha.php``.

6. Change the config option on line 12 to **recaptcha**.

7. Copy **Site key** and **Secret key** from Google ReCaptcha page and inserte it on line number 51 and 52 respectively as shown in below image

.. image:: images/pp_key.png
 
J. To verify Recpatcha, visit the user registration page in NADA and verify that you can see the reCaptcha similar to the screenshot below.

.. image:: images/varify_captcha.png

