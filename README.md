# Reporta-apps-and-backend-db
Code for the iOS and Android versions of Reporta mobile apps as well as the backend database server.

We’ve posted separate files containing code for both the iOS and Android versions of the app as well as the backend server.  All code has been released under GPL 3 and users are free to review, comment and reuse the code any way they like.

We’d love to hear your comments and suggestions on how to improve the code and additional features you’d like to see in it.  
All we ask is that comments and contributions be reasonably respectful and made in the spirit of improving Reporta and the functions is provides users.

We will absolutely take them to heart as we work on future releases.

**************************************************************************************

One of the things we're most interested in exploring is the best data encryption methodology for the mobile apps and their connection back to the server. The initial release of the apps, and this public release, primarily deploy iOS's and Android's native encryption. We've tweaked it in this public release based on feedback received from our circle of advisers and others in the digital freedom community.

We've had numerous discussions regarding the best encryption implementation possible within Reporta's use case. That use case presents two big challenges for implementing encryption. First is the need for a remote server--the app MUST use the backend server so that alerts can be sent even if a user's phone is unavailable. When conducting our user research we consistently heard from journalists in the field that when being harassed, their phone is almost always taken from them. So moving the alert process off the phone to the server is critical to the app's effectiveness.

The second challenge is that Reporta must be able to send alerts in clear text so recipients don't need a client to decrypt any alerts the app sends when a journalist is in danger. So point to point encryption (which is almost always the best solution from a pure security perspective) just isn't a workable approach.

So you can see that implementing encryption on the app is not simple. While there are lots of options, no approach arose in discussions that appeared superior, given our use case, the the native encryption tools.

We're VERY interested in seeing if others, once they've taken a look at things, have some useful suggestions

***************************************************************************************


What’s in the public code?

Reporta has been updated since the initial launch to reflect all the suggestions that folks made after we launched Reporta.  In addition, we've revised Reporta's Privacy Policy and Terms of Service to reflect those changes. There’s a link to the new Privacy Policy on www.reporta.org

It's taken a little longer than we had hoped to get this code posted-- but we have taken time to consult a number of advisors as we've been enhancing Reporta and everyone we've consulted advised that we make and test all the code changes BEFORE we release the code publically.  
That approach makes a lot of sense--  if only because we want folks who download and look at Reporta's code to have the most up-to-date version.
Here’s a list of changes users will see in the app versus the 1.0 version we launched in October.
  
-All analytics and crashlytics removed from the app as well as the backend database
  -Enhanced encryption of data on the user's phone as well as more aggressive deletion of data from the phone once it's no longer needed to run the app
  
-Enhanced encryption of data on the backend server
  -Revised data retention procedures that delete all server data related to an alert or check-in as soon as that activity is completed. 

-Improvements to translations
  
-Lots of smaller tweaks to the apps run more smoothly and minimize data collected

We encourage you to provide us your feedback and thoughts about the project. Feel free to leave comments via the Github project page or email them to us directly at techfeedback@reporta.org

