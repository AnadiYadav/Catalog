# Catalog
**Prerequisites**
To run this project, you need to have Node.js installed on your system.

Step 1: Install Node.js
Download Node.js:

Visit the official Node.js download page.
Download the LTS (Long-Term Support) version for your operating system.
Install Node.js:

Run the installer you downloaded and follow the setup instructions.
Ensure the Node.js installer includes the npm (Node Package Manager) option.
Verify Installation:

Open a terminal or command prompt and type the following commands to verify the installation:
node -v
npm -v
This should output the installed versions of Node.js and npm.
Step 2: Clone the Project
Clone this repository to your local machine or download the files manually.
Step 3: Prepare the JSON Input
The project uses a JSON file (input.json) to store test data.
If you'd like to change the test case:
Modify the values in input.json to fit your requirements. Here's an example structure:
{
    "keys": {
        "n": 9,
        "k": 6
    },
    "1": {
        "base": "10",
        "value": "28735619723837"
    },
    "2": {
        "base": "16",
        "value": "1A228867F0CA"
    },
    ...
}

2. After making changes to the JSON data, ensure that you also update the file path in the JavaScript code.
Open the JavaScript file and update the require() function to point to the correct file:
const inputJson = require("./input.json"); // Change the path if necessary

Step 4: Run the Code
Open a terminal or command prompt in the project directory.
Run the program using Node.js:
node your-script-name.js
The program will read the data from the JSON file, process it, and perform Lagrange interpolation to estimate the value at xi = 0.
# Modifying the Test Case
Change the JSON file: If you wish to modify the test data, you can edit the input.json file with new values and bases.
Change the file path: After editing the file, make sure the JavaScript code is pointing to the correct file path (as shown in Step 3).
