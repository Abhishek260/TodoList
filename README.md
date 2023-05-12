# TodoList
The code provided is an HTML document that creates a simple TODO list application. Here's a breakdown of its structure and functionality:
The document starts with the usual HTML doctype declaration and the opening <html> tag.
The <head> section contains meta tags for character encoding and viewport settings. It also includes a link to the Bootstrap CSS framework for styling.
The title of the page is set to "TODOs List" using the <title> tag.
The <body> section begins with a container <div> for the main content.
Inside the container, there is a <h2> heading that displays "TODO's List" in the center of the page.
Below the heading, there are two form elements within separate <div> containers. The first is an input field for the item title, and the second is a textarea for the item description.
After the form elements, there are two buttons: "Insert into list" and "Delete list". The "Insert into list" button triggers the getAndUpdate() function when clicked, and the "Delete list" button triggers the clearStorage() function when clicked.
The next <div> container with the id "items" is used to display the list of TODO items. It contains a <h2> heading with the text "Your Items" and a <table> element with the class "table".
Inside the table, there is a <thead> section with table headers for "Sr.No", "Title", "Description", and an empty header cell.
The <tbody> section with the id "tableBody" is used to dynamically populate the table rows with TODO items. Currently, it contains a static row with placeholder data.
The JavaScript code is enclosed within the <script> tags. It defines several functions to handle the functionality of the TODO list.
The getAndUpdate() function is responsible for retrieving the input values from the form, storing them as an array in the browser's local storage, and updating the list.
The update() function retrieves the array from the local storage, generates the HTML for the table rows based on the array data, and updates the table with the dynamic content.
The add variable is assigned the reference to the "Insert into list" button element. An event listener is added to this button, which calls the getAndUpdate() function when clicked.
The deleted(itemIndex) function deletes the item at the specified index from the array stored in the local storage, updates the local storage and the table accordingly.
The clearStorage() function prompts the user for confirmation and then clears the local storage and updates the table.
The empty() function is used to clear the input fields after the user clicks the "Insert into list" button.
Finally, the JavaScript code calls the update() function to initialize the list with any existing items in the local storage.
Overall, this code provides a basic implementation of a TODO list application that allows users to add items, delete items, and clear the list using browser local storage for data persistence. The Bootstrap CSS framework is used for styling the components.
Project by Coding Ninjas
