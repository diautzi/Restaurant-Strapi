# Strapi application

A quick description of your strapi application:

1. Install Strapi and Create a new project
yarnnpx
yarn create strapi-app my-project --quickstart

#2. Create an Administrator user
Navigate to http://localhost:1337/admin.

Complete the form to create the first Administrator user.
Click Ready to start.

#3. Create a Restaurant Content Type
Navigate to PLUGINS - Content Type Builder, in the left-hand menu.

Click the "+ Add Content Type" link
Enter restaurant, and click Done
A window opens with fields options:
Click the String field
Type name in the Name field
Click over to the ADVANCED SETTINGS tab, and check the Required field and the Unique field
Click the "+ Add New Field" button
Click the Rich Text field
Type description under the BASE SETTINGS tab, in the Name field
Click Done
Click the Save button and wait for Strapi to restart

#4. Create a Category Content type
Navigate back to PLUGINS - Content Type Builder, in the left-hand menu.

Click the "+ Add Content Type" link
Enter category, and click Done
A window opens with fields options:
Click the String field
Type name under the BASE SETTINGS tab, in the Name field
Click over to the ADVANCED SETTINGS tab, and check the Required field and the Unique field
Click the "+ Add New Field" button
Click the Relation field
On the right side, click the Permissions dropdown and select, Restaurant
In the center, select the icon that represents many-to-many. The text should read, Categories has and belongs to many Restaurants
Click Done
Click the Save button and wait for Strapi to restart

#5. Add content to "Restaurant" Content Type
Navigate to CONTENT TYPES - Restaurants, in the left-hand menu.

Click on + Add New Restaurant button. Type Biscotte Restaurant in the Restaurant field. Type Welcome to Biscotte restaurant! Restaurant Biscotte offers a cuisine based on fresh, quality products, often local, organic when possible, and always produced by passionate producers. into the Description field.
Click Save.
You will see your restaurant listed in the entries.

#6. Add categories to the "Category" Content Type
Navigate to CONTENT TYPES - Categories.

Click on + Add New Category button. Type French Food in the Category field. Select Biscotte Restaurant, on the right, from Restaurant (0)
Click Save.
You will see the French Food category listed in the entries.

Click on + Add New Category button. Type Brunch in the Category field. DO NOT ADD IT HERE to Biscotte Restaurant.
Click Save.
You will see the Brunch category listed in the entries.

Navigate back to CONTENT TYPES - Restaurants.

Click on Biscotte Restaurant
On the right, under Categories(1), select the Add an item..., and add Brunch as a category for this restaurant, and click the Save button.
You have now seen two different ways to use the relation field type to add and connect relations between Content Types.

#7. Set Roles and Permissions
Navigate to PLUGINS - Roles & Permissions.

Click the Public Role.
Scroll down under Permissions, find Restaurant. Click the checkbox next to find and findone.
Repeat and find Category. Click the checkbox next to find and findone.
Click Save.
#8. Consume the Content Type's API
Here we are! The list of restaurants is accessible at http://localhost:1337/restaurants.

CONGRATULATIONS

👏 Congratulations, you have now completed the Strapi Quick Start. Where to go next?

Learn how to use Strapi with React (Gatsby or Next.js) or Vue.js (Nuxt.js).
Read the concepts and do the Tutorial to deep dive into Strapi.
Get help on StackOverflow.
Read the source code, contribute or give a star on GitHub.
Follow us on Twitter to get the latest news.
Join the vibrant and active Strapi community on Slack.
