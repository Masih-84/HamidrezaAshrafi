# HamidrezaAshrafi
Part 3- The final Task(25) of the Hyperion boot-camps course 
import subprocess

# Clone the repository
subprocess.run(["git", "clone", "https://github.com/Masih-84/HamidrezaAshrafi.git"])

# Navigate to the cloned repository
subprocess.run(["cd", "HamidrezaAshrafi"])

# Create the HTML file
html_content = '''
<!DOCTYPE html>
<html>
<head>
    <title>Landing Page</title>
    <style>
        /* Add your custom CSS styles here */
    </style>
</head>
<body>
    <h1>Welcome to My Landing Page</h1>
    <img src="path-to-your-image.jpg" alt="Description of the image">
    <!-- Add more content here -->
</body>
</html>
'''

# Save the HTML content to a file
with open("HamidrezaAshrafi/index.html", "w") as file:
    file.write(html_content)

# Commit and push the changes
subprocess.run(["git", "add", "."])
subprocess.run(["git", "commit", "-m", "Added landing page content"])
subprocess.run(["git", "push", "origin", "main"])
