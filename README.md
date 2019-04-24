# ReactWPTheme

This is a test how to create React WordPress theme on top of WordPress backend.
The tool I use is create-react-wptheme and can be found from: https://www.npmjs.com/package/create-react-wptheme


# Usage

To create a WordPress theme using the create-react-wptheme, follow these steps.

Make sure your WordPress server is up and running.  
Change dir into your WordPress themes folder (this is just an example, use your real themes folder).  
Windows: cd C:\xampp\htdocs\wordpress\wp-content\themes 
Mac or *nix: cd /xampp/htdocs/wordpress/wp-content/themes  
Use npx create-react-wptheme to make a new theme 
For example: (replace "my_react_theme" with whatever you want your theme to be named):  
npx create-react-wptheme my_react_theme  
If you want to use TypeScript, then the command would be:  
npx create-react-wptheme my_react_theme --typescript  
When it finishes it'll tell you to change into your new theme's folder and run the Nodejs watcher (replace "my_react_theme"  with the same name you used in the previous step):  
cd my_react_theme/react-src  
npm run wpstart 
That sets up the theme so that it can be seen in the WordPress admin area.  
Go there now and set your WordPress site to use this theme.  
View the site in your browser with the new theme.  
You must do this as it does some extra setup via PHP.  
If you get PHP errors, most likely your web server doesn't have write access to your theme.  
Write access for your web server is only needed during this setup step.  
You can revoke write access after the setup has completed.  
Interested (paranoid?) about what it's doing? Check out the file: <your theme folder name>/index.php  
When that's done the theme tells you to Please restart the Nodejs watcher now...  
To do that, go back to your command prompt where you first ran npm run wpstart and rerun that same command again.  
In a few seconds you should see your browser load with the standard create-react-app page, but it's running as a WordPress  theme!  
