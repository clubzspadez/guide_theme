# How to run this project(MACos)

## Setting up local theme preview

### To set up local theme preview

1. If not already done, enable API access in your Zendesk Support account by going to Admin > Channels > API.
2. Install the Zendesk apps tools (ZAT).
   See Installing and using the Zendesk apps tools in the Develop Help Center.

   - [Installing ZAT](https://develop.zendesk.com/hc/en-us/articles/360001075048)

3. If you previously installed ZAT to build Zendesk apps, make sure to update it by running the following command in your command-line interface:
   ```
   $ gem update zendesk_apps_tools
   ```

## Starting local theme preview

https://support.zendesk.com/hc/en-us/articles/115012793547-Previewing-theme-changes-locally-Guide-Professional-and-Enterprise-

You should start local theme preview before you start working on theme files on your computer.

To start local theme preview

1. In your command line interface, navigate to the folder containing the exported and unzipped theme files.
   Use the cd command (for change directory) to navigate to a child folder. Example:

```
$ cd guide_themes/newlook_theme
```

To back up one directory, use cd followed by a space and two periods. Example:

```
cd ..
```

2. Run the following command:

```
$ zat theme preview
```

At the prompts, enter your Zendesk Support subdomain, as well as the email and password you use to sign in to Zendesk Guide.

The subdomain and email are saved in a text file named .zat in the theme's folder so that you only need to enter your password the next time you start preview mode. If you make a mistake entering your username or password, delete the .zat file and start again. Note that files with leading periods are hidden in macOS by default. See Show Hidden Files in Mac OS X on the osxdaily.com website.

If you use single sign-on (SSO) to sign in to Guide (such as using Google or Microsoft credentials), you can sign in using an API token that you can get from the Support admin interface. See API token in the REST API docs. When prompted by ZAT to sign in, enter {your_email}/token for your user name, where "/token" is the actual string "/token". Use the actual API token for your password. Example:

```
Enter your username: jdoe@example.com/token
Enter your password: e8Pvy0pvGzE8meUQxWgjIYkjr
```

After successfully signing in, preview mode starts and runs in the background:

3. Copy the "Ready" URL in the output and paste it in a browser.
   In the example, the URL is https://nadosolutions.zendesk.com/hc/admin/local_preview/start.

An unformatted page loads after you sign in. Modern browsers have a security feature that blocks certain local files (known as mixed content) from loading in a page. You can disable the feature in Chrome and Firefox as described in the following step.

In Chrome or Firefox, click the shield icon in the Address bar and agree to load an unsafe script (Chrome) or to disable protection on the page (Firefox). In Firefox, the shield icon is located on the left side of the Address bar.
