WPF app that let you stores you favourite recipes

Tanaka Gavaza st10399462

The RecipeApp was created to help home cooks manage their recipes with ease, making cooking a delightful and hassle-free experience. In today's fast-paced world, people often struggle to keep track of their favorite recipes, find it challenging to adjust ingredient quantities when cooking for different numbers of guests, or need a straightforward way to store and access their recipes.

With RecipeApp, users can quickly enter their recipes, scale them based on the number of servings required, reset the recipes to their original state, and even clear the data to enter new recipes. The intuitive console menu makes it simple for users to interact with the application and perform various tasks related to their recipes.


how this program works

1. The program starts by displaying a menu of options.
2. Based on the user's choice, the program executes the corresponding action:
   	Option 1: Add Recipe:
	The program prompts you to provide the recipe name and then guides you to enter the number of ingredients, ingredient details, and steps for the recipe.	
	It creates a new Recipe object with the provided information, adds it to the Recipes dictionary, and displays a success message.

Option 2: Display all recipes:
	The program checks if there are any recipes in the Recipes dictionary. If not, it displays an error message.
	If recipes exist, it sorts the recipe names in alphabetical order and displays each recipe's details, including total calories.
	The DisplayRecipe and TotalCalories methods of the Recipe class are used to format and calculate the recipe information.

Option 3: Display a specific recipe:
	The program checks if there are any recipes in the Recipes dictionary. If not, it displays an error message.
	If there are recipes, it prompts you to enter the name of the recipe you want to display.
	If the entered recipe name exists in the Recipes dictionary, it displays the recipe's details and total calories.
	If the entered recipe name does not exist, it displays an error message.

Option 4: Scale a recipe:
	The program checks if there are any recipes in the Recipes dictionary. If not, it displays an error message.
	If recipes exist, it prompts you to confirm your intention to scale a recipe.
	If you confirm, it prompts you to enter the name of the recipe you want to scale and the scaling factor (0.5, 2, or 3).
	If the entered recipe name exists in the Recipes dictionary and the scaling factor is valid, it scales the recipe using the ScaleRecipe method of the corresponding Recipe object.
	It then displays the updated recipe details and total calories.

Option 5: Reset a recipe:
	The program checks if there are any recipes in the Recipes dictionary. If not, it displays an error message.
	If recipes exist, it prompts you to confirm your intention to reset a recipe.
	If you confirm, it prompts you to enter the name of the recipe you want to reset.
	If the entered recipe name exists in the Recipes dictionary, it resets the recipe to its original state using the ResetRecipe method of the corresponding Recipe object.
	It then displays the original recipe details and total calories.
Option 6: Add to menu
	Add recipes to the menu: The user can select a recipe from a dropdown menu and add it to the menu. The selected recipe's ingredients and total calories are displayed in a list.
	Calculate total calories: When a recipe is added to the menu, the application calculates the total calories for that recipe and displays a message if the calorie limit is exceeded.
	Generate a pie chart: The user can click the "Create Pie Chart" button to generate a pie chart showing the distribution of food groups in the chosen recipes.
	Food group counting: The application counts the number of ingredients in each food group for the chosen recipes and updates the pie chart accordingly.
	Dependencies
	LiveCharts: This application uses the LiveCharts library to create and display the pie chart. Make sure to include the necessary dependencies in your project.	

Option 7: Clear all recipes:
	The program checks if there are any recipes in the Recipes dictionary. If not, it displays an error message.
	If recipes exist, it prompts you to confirm your intention to clear all recipes.
	If you confirm, it clears the Recipes dictionary and displays a success message.

Option 8: Exit the program:
	When you choose this option, the program sets the exit variable to -1, indicating the termination of the program.
	The program then terminates, and the console application closes.
3. After executing an action, the program returns to the main menu until the user chooses to exit.
