# How to run this project(MACos)

## Setting up local theme preview

### To set up local theme preview

1. If not already done, enable API access in your Zendesk Support account by going to Admin > Channels > API.
2. Install the Zendesk apps tools (ZAT).
   See Installing and using the Zendesk apps tools in the Develop Help Center.

   ### Installing ZAT

   Note: If you're using macOS or Ubuntu and any of the following commands complains that you don't have write permissions for a directory, start the command with sudo to request admin privileges, then enter the password for your system when prompted. Example: $ sudo gem install rake.

3. First, install rake, a build automation tool, with the following command in your command-line interface:

$ gem install rake

2. Next, install ZAT with the following command:

$ gem install zendesk_apps_tools

3. The ZAT gem and a number of supporting gems are installed, along with related documentation.

Updating ZAT

4. Zendesk updates ZAT from time to time. To get the latest version, run the following command:

$ gem update zendesk_apps_tools

3. If you previously installed ZAT to build Zendesk apps, make sure to update it by running the following command in your command-line interface:
   $ gem update zendesk_apps_tools

#Starting local theme preview
https://support.zendesk.com/hc/en-us/articles/115012793547-Previewing-theme-changes-locally-Guide-Professional-and-Enterprise-
