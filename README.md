You have been hired by a local restaurant to **extend** the backend system for managing their online menu. In addition to creating and reading menu items, the restaurant needs the following functionality:

- **Update existing menu items** in the database.
- **Delete menu items** that are no longer needed or are discontinued.

### Instructions

### Initialize the Project:

Basic express template was given  
You need to install all the necessary packages required for the task.

### Define a MenuItem schema that includes:
- name (String, required)
- description (String)
- price (Number, required)

### MongoDB Atlas Connection

- Create a MongoDB Atlas account and set up a free cluster.
Use Mongoose to connect your Express server to the MongoDB Atlas cluster.


 **Implement Update & Delete**  
   - **PUT /menu/:id**: Updates an existing menu item.  
     - Accepts `name`, `description`, and `price` (or any subset) in the request body.
     - Responds with the updated object (or an error message if something goes wrong).

   - **DELETE /menu/:id**: Deletes an existing menu item.  
     - Responds with a success message if the item is deleted (or an error if the `id` is invalid or not found).

 **Error Handling & Validation**  
   - Validate incoming data to ensure required fields are not empty.
   - Respond with a descriptive error message if the item cannot be updated or deleted.

 **Testing**  
   - Use Postman (or a similar tool) to test:
     - **PUT** requests to update an existing menu item.
     - **DELETE** requests to remove a specific menu item.



# **How to Fork and Set Up Your Repository**

---

## **1. Fork the Repository on StackBlitz**

- You will be provided with a **StackBlitz** link for the assignment.
- Open the link in your browser and click on the **Fork** button in StackBlitz.  
  This will create a copy of the repository in your StackBlitz account.

---

## **2. Clone the Repository to Your Personal GitHub**

- After forking, you can download the project or push it directly to your personal GitHub repository:
  - **Option 1: Download and Push**
    1. Download the repository files from StackBlitz.
    2. Open your terminal/command prompt, navigate to the project folder, and run:
       ```bash
       git init
       git remote add origin <your_github_repo_url>
       ```
       Replace `<your_github_repo_url>` with your personal GitHub repository URL.
    3. Commit and push the files to your GitHub repository:
       ```bash
       git add .
       git commit -m "Completed the assignment"
       git push -u origin main
       ```
  - **Option 2: Push Directly**
    1. Use the **Push to GitHub** option in StackBlitz to directly connect and push the repository to your GitHub account.

---

## **3. Submission Instructions**

- Once your code is successfully pushed to GitHub:
  1. Copy the link to your GitHub repository.
  2. Submit the link on the assignment submission portal.  
     The link should follow this format:  
     **`https://github.com/<your_username>/<repository_name>`**

---

### **Example Submission**

If your GitHub username is `johnDoe` and the repository name is `assignment-repo`, the submission link would look like this:  
**`https://github.com/johnDoe/assignment-repo`**
