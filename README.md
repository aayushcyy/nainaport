💨 How to Add Tailwind CSS to a Regular HTML Project (Tailwind v4)

🧩 Step-by-Step Setup

1️⃣ Initialize Your Project
run this command in root dir

    "npm init -y"

2️⃣ Install Tailwind CSS
run

"npm install -D tailwindcss"

3️⃣ Create Folders
create a folder in your root dir called dist by running

"mkdir dist"

4️⃣ Set Up Tailwind
create a new folder called src with file inside called input.css and add this line into that file

"@import "tailwindcss";"

5️⃣ Configure Your Scripts
Open your package.json and replace or add the "scripts" section with this:

"scripts": {
"build": "tailwindcss -i ./src/input.css -o ./dist/output.css",
"watch": "tailwindcss -i ./src/input.css -o ./dist/output.css --watch"
}

6️⃣Link Tailwind in Your HTML
link the output.css file in <head> tag

"<link rel="stylesheet" href="../dist/output.css" />"

7️⃣Run Tailwind
run
"npm run watch"
